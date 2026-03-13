# Implementación de Centralización de Datos de Usuario y Protección de Archivos

## 🎯 Justificación Técnica
Para garantizar la integridad de la información y facilitar la gestión de backups, este proyecto establece la transición del almacenamiento local al almacenamiento centralizado en servidor. Esto mitiga el riesgo de pérdida de datos por avería de hardware en los puestos finales y optimiza el RTO (Recovery Time Objective).

---

## 🛠️ Arquitectura del Servicio de Archivos

### 1. Redirección de Carpetas mediante GPO
Se implementa una política de grupo para redirigir las carpetas críticas de usuario (`Escritorio` y `Documentos`) a un recurso compartido en red de forma transparente para el usuario.

* **Configuración GPO:** `Configuración de usuario` > `Directivas` > `Configuración de Windows` > `Redirección de carpetas`.
* **Ruta UNC de destino:** `\\SRV-STORAGE-01\UserShares$\%username%`
* **Parámetros:** Se habilita la transferencia de contenidos y se otorga permiso exclusivo al usuario y al sistema.

### 2. Gestión de Cuotas y Filtros (FSRM)
Utilizando **File Server Resource Manager**, se establecen controles para evitar el uso indebido del almacenamiento corporativo:

* **Cuotas de Almacenamiento:** Límite de 5GB por usuario (aviso al 85%, bloqueo al 100%).
* **Filtros de Archivos (Anti-Ransomware):** Bloqueo activo de extensiones de archivos no permitidas (ejecutables, archivos temporales, extensiones de cifrado conocidas).

### 3. Alta Disponibilidad de Datos con VSS
Se activa **Volume Shadow Copies (VSS)** en los volúmenes de datos para permitir la recuperación de versiones previas por parte de los propios usuarios sin intervención de IT.

* **Programación:** Capturas de estado a las 08:00h y 14:00h diariamente.
* **Retención:** Configuración de espacio dedicado para el histórico de versiones.

---

## 📋 Prerrequisitos de Implementación

1.  **Directorio Activo:** Los usuarios deben pertenecer a la Unidad Organizativa (OU) sobre la que se vincula la GPO.
2.  **Permisos NTFS:** * Carpeta raíz: `SYSTEM` (Control Total), `Administradores` (Control Total).
    * Subcarpetas de usuario: `%username%` (Control Total - Creador/Propietario).
3.  **Rutas UNC:** Es crítico el uso de nombres DNS en lugar de IPs para mantener la persistencia ante cambios de infraestructura.

---

## 🚀 Plan de Despliegue
1.  Creación de recursos compartidos con permisos de "Usuarios Autenticados".
2.  Configuración de la plantilla de cuotas en FSRM.
3.  Vinculación de la GPO de redirección en modo de prueba para un grupo de control.
4.  Ejecución de `gpupdate /force` en los puestos finales para iniciar la migración de datos local-servidor.

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/SysAdmin-Playbooks/readme.md/)

---
