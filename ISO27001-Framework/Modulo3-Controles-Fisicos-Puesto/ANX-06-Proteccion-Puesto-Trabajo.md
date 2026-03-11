# Anexo 6: Protección del Puesto de Trabajo

## 🎯 Objetivo
Garantizar la seguridad de toda la información y los recursos gestionados desde el puesto de trabajo, minimizando los riesgos de acceso no autorizado, pérdida de datos o compromiso de la integridad de los sistemas.

---

## 🛡️ Normativa de Protección del Puesto de Trabajo

La organización dispone de una normativa específica que recoge las medidas necesarias para proteger el puesto de trabajo. Esta normativa se revisa periódicamente para adaptarse a cambios tecnológicos o nuevos servicios contratados.

### 1. Control y Configuración Técnica (Responsabilidad de IT)
* **Bloqueo Programado de Sesión:** Se configurará mediante GPO el bloqueo automático de sesión tras un periodo breve de inactividad. Se recomienda además el apagado programado de estaciones de trabajo al finalizar la jornada para optimizar el consumo y la seguridad.
* **Actualizaciones y Salud del Sistema:**
    * Mantenimiento estricto del Sistema Operativo actualizado.
    * Antivirus activo, monitorizado y con firmas actualizadas.
* **Control de Periféricos:** Deshabilitación por defecto de puertos USB en dispositivos que no requieran su uso por funciones específicas de su puesto.
* **Seguridad en Impresoras y Equipos Auxiliares:**
    * Ubicación dentro del perímetro del cortafuegos (Firewall).
    * Acceso al panel de gestión mediante credenciales robustas y canales cifrados.
    * Configuración de seguridad en redes Wi-Fi integradas.
    * Deshabilitación de conectores USB físicos no críticos.

### 2. Gestión de Medios de Almacenamiento
El personal debe aplicar la normativa relativa al uso de:
* Almacenamiento local (restringido a archivos temporales).
* Almacenamiento en red corporativa (prioritario para backups).
* Almacenamiento en la nube autorizada.
* Dispositivos extraíbles (sujetos a cifrado y autorización).

### 3. Integridad del Puesto de Trabajo
Queda estrictamente prohibida la alteración de la configuración del equipo o la instalación de software no autorizado. Cualquier necesidad técnica debe ser escalada al departamento de IT mediante los canales oficiales de solicitud.

---

## 📋 Política de Mesas Limpias y Despacho Seguro

El compromiso con la seguridad incluye la gestión del entorno físico:
* **Orden y Limpieza:** Mantener el puesto de trabajo libre de documentación sensible al ausentarse.
* **Custodia de Información:** Guardar documentos y dispositivos extraíbles en cajoneros o armarios con llave al finalizar la jornada.
* **Gestión de Credenciales:** Prohibición estricta de anotar usuarios o contraseñas en soportes físicos (post-it, cuadernos, etc.).
* **Equipos de Reproducción:** Recogida inmediata de documentos en impresoras o escáneres. No abandonar documentación sensible en las bandejas de salida.

---

## ⚠️ Notificación de Incidentes de Seguridad

Es obligación de todo el personal notificar de inmediato cualquier anomalía, incluyendo:
* Alertas de malware o comportamiento extraño del sistema.
* Intentos de ingeniería social (llamadas o correos sospechosos).
* Pérdida o robo de dispositivos (portátiles, móviles, USB).
* Borrado o alteración accidental de información crítica.
* Detección de personal no identificado en áreas restringidas.

---

## ✅ Checklist de Control

| Nivel | Alcance | Control | Estado |
| :--- | :--- | :--- | :---: |
| **B** | **PRO** | Difusión de normativa y auditorías de cumplimiento. | ☐ |
| **A** | **TEC** | Implementación de bloqueo automático por GPO. | ☐ |
| **B** | **TEC** | Gestión de actualizaciones (Patch Management). | ☐ |
| **B** | **TEC** | Deshabilitación de puertos USB por política. | ☐ |
| **B** | **PER** | Cumplimiento de Política de Mesas Limpias. | ☐ |
| **B** | **PER** | Uso de contraseñas robustas (Min. 8 caracteres, complejidad). | ☐ |
| **B** | **PER** | Obligación de bloqueo manual al levantarse del puesto. | ☐ |
| **A** | **PER** | Aplicación de cifrado en información confidencial. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________
