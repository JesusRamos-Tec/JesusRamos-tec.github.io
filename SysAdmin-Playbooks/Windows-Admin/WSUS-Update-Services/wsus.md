# 🔄 Gestión Centralizada de Actualizaciones: WSUS

Este laboratorio documenta el despliegue y la configuración de **Windows Server Update Services (WSUS)** en un entorno de dominio para la gestión controlada de parches de seguridad y actualizaciones de sistema.

> [!IMPORTANT]
> **Nota sobre el ciclo de vida:** Aunque Microsoft ha anunciado la deprecación de WSUS para priorizar soluciones en la nube, su implementación sigue siendo un estándar crítico en infraestructuras *on-premise* y entornos con restricciones de ancho de banda.

---

## 🏗️ Fase 1: Instalación del Rol de Servidor

1. **Agregar Rol:** Desde el Administrador del Servidor, iniciamos el Asistente para "Agregar roles y características".
2. **Tipo de Instalación:** Seleccionamos "Instalación basada en características o en roles".
3. **Selección de Servidor:** Confirmamos nuestro servidor de destino en el grupo de servidores.
4. **Rol WSUS:** Marcamos "Windows Server Update Services" y aceptamos la instalación de las características requeridas.
5. **Configuración de Almacenamiento:** Definimos una ruta local o de red (se recomienda un disco dedicado) para almacenar físicamente las actualizaciones.
6. **Instalación:** Pulsamos "Instalar" y, una vez finalizado, ejecutamos las **"Tareas posteriores a la instalación"** desde la bandera de notificaciones del Server Manager.

---

## ⚙️ Fase 2: Configuración del Servicio

1. **Asistente de Configuración:** Abrimos la consola de WSUS desde Herramientas Administrativas.
2. **Origen de Sincronización:** Seleccionamos "Sincronizar desde Microsoft Update".
3. **Servidor Proxy:** Configuramos los datos si la red lo requiere; de lo contrario, omitimos este paso.
4. **Productos y Clasificaciones:** - Escogemos los sistemas operativos presentes en nuestra red (ej. Windows 10, Windows 11, Windows Server 2022).
   - Seleccionamos los tipos de parches (Seguridad, Críticos, Definiciones).
5. **Sincronización Inicial:** Realizamos una sincronización manual inicial para poblar la base de datos de actualizaciones disponibles.

---

## 🛰️ Fase 3: Despliegue mediante Directivas de Grupo (GPO)

Para que los equipos se reporten al servidor WSUS, configuramos una GPO en el Controlador de Dominio:

### 1. Creación de la GPO
Creamos y vinculamos una nueva GPO (ej. `SRV_WSUS_Updates`) a la Unidad Organizativa de los equipos.

### 2. Parámetros Críticos (Configuración de Equipo)
Navegamos a: `Configuración del equipo` > `Plantillas administrativas` > `Componentes de Windows` > `Windows Update`.

* **Configurar Actualizaciones Automáticas:** Habilitamos y seleccionamos el comportamiento deseado (ej. Opción 4: Descargar automáticamente y programar instalación).
* **Especificar ubicación del servicio Windows Update en la intranet:**
    - **Servidor de actualización:** `http://NombreServidor.dominio.local:8530`
    - **Servidor de estadísticas:** `http://NombreServidor.dominio.local:8530`
* **Habilitar destinatarios del lado cliente:** Habilitamos y definimos el nombre del grupo (ej. `Equipos_Produccion`) para organizar los PCs en la consola de WSUS.

---

## 🔍 Fase 4: Troubleshooting (Depuración de Errores)

Si un equipo cliente no aparece en la consola de administración, seguimos este protocolo de pruebas:

1. **Test de Conectividad:** Desde el navegador del cliente, intentamos descargar: `http://NombreServidor.dominio.local:8530/iuident.cab`. Si descarga, la comunicación web es correcta.
2. **Forzar Políticas:** Ejecutamos `gpupdate /force` en el CMD del cliente.
3. **Forzar Reporte:** Ejecutamos los comandos para forzar la detección inmediata:
   ```cmd
   wuauclt.exe /detectnow /reportnow
   ```
4. **Verificación de RSoP:** Usamos la herramienta rsop.msc para confirmar visualmente qué políticas de Windows Update están ganando prioridad en el sistema.
5. **Diagnóstico GPResult:** Generamos un informe detallado de directivas para asegurar que el equipo está leyendo la GPO de WSUS:
   ```cmd
   gpresult /v > gpresult_wsus.txt
   ```

   ---

## 🛡️ Best Practices (Buenas Prácticas de Administración)

Implementar WSUS requiere una estrategia de mantenimiento para evitar la saturación del servidor y fallos en los clientes:

* **Estrategia de Grupos (Anillos):** Nunca apruebes actualizaciones para toda la empresa a la vez. Crea un grupo de Test con equipos de IT, espera 48-72h y, si no hay fallos, aprueba para Producción.
* **Limpieza de Servidor:** Ejecuta el "Asistente para la limpieza del servidor" mensualmente para eliminar actualizaciones caducadas y archivos innecesarios.
* **Aprobación de Definiciones:** Configura reglas de Aprobación Automática para las "Actualizaciones de definiciones" (Antivirus/Defender), ya que son críticas y constantes.
* **Monitorización de Disco:** Vigila el tamaño de la carpeta WsusContent. WSUS puede consumir cientos de GB rápidamente si se seleccionan demasiados productos.

---

## ⬅️ Navegación
[Volver al Índice SysAdmin-Playbooks](https://jesusramos-tec.github.io/SysAdmin-Playbooks/)

---
