# Anexo 19: Seguridad en Aplicaciones y Portales Web

## 🎯 Objetivo
Garantizar la protección de los activos web de la organización, asegurar la confidencialidad de los datos de los usuarios mediante el cumplimiento del RGPD y mitigar riesgos de intrusión, desfiguración (defacement) o robo de información.

---

## 🔐 Protección de Datos y Cumplimiento (RGPD/LSSI)
Cualquier portal web que recoja datos de carácter personal debe cumplir estrictamente con:
* **Principio de Minimización:** Solicitar únicamente los datos estrictamente necesarios.
* **Consentimiento Explícito:** Implementar "checkboxes" no marcados por defecto para la aceptación de políticas.
* **Transparencia:** Publicar y mantener actualizados el **Aviso Legal**, la **Política de Privacidad** y la **Política de Cookies**.
* **Derechos ARCO+:** Facilitar mecanismos claros para que los usuarios ejerzan sus derechos de acceso, rectificación, supresión y portabilidad.

---

## 🛠️ Seguridad en la Infraestructura (Hosting)

### Escenario A: Alojamiento Interno (On-Premise)
* **Segmentación (DMZ):** El servidor web debe estar ubicado en una zona desmilitarizada (DMZ), aislado de la red de datos interna.
* **Perímetro:** Protección mediante Firewall de Aplicación Web (WAF) y sistemas de detección/prevención de intrusos (IDS/IPS).
* **Hardening:** Deshabilitación de servicios innecesarios (FTP sin cifrar, listado de directorios, servicios de gestión remota no seguros).



### Escenario B: Alojamiento Externo (Cloud/Hosting)
* **Acuerdos de Nivel de Servicio (SLA):** El contrato debe garantizar disponibilidad, copias de seguridad gestionadas y parches de seguridad.
* **Propiedad del Código:** Cláusula de propiedad intelectual sobre el código fuente y las bases de datos.
* **Auditoría de Terceros:** Derecho a solicitar informes de seguridad o registros de actividad de los administradores del proveedor.

---

## 🛡️ Aseguramiento del Gestor de Contenidos (CMS)
Para plataformas como WordPress, Joomla o desarrollos a medida, se aplicarán las siguientes medidas de "Hardening":
1.  **Cifrado:** Instalación obligatoria de certificados **SSL/TLS (HTTPS)** de confianza.
2.  **Gestión de Accesos:** * Eliminación del usuario "admin" por defecto.
    * Uso de contraseñas robustas y Doble Factor de Autenticación (MFA) para el panel de administración.
    * Implementación de CAPTCHA en todos los formularios para evitar spam y ataques de fuerza bruta.
3.  **Mantenimiento:** * Eliminación de módulos, plugins o plantillas no utilizados.
    * Borrado de directorios de instalación y archivos `readme.html` que revelen versiones del software.
    * Actualización inmediata de parches de seguridad del Core y complementos.



---

## ✅ Checklist de Control

| Nivel | Alcance | Control | Estado |
| :--- | :--- | :--- | :---: |
| **A** | **PRO/TEC** | Certificado SSL/TLS activo y configurado (HTTPS). | ☐ |
| **A** | **PRO/TEC** | Textos legales y gestión de consentimiento conformes al RGPD. | ☐ |
| **B** | **PRO/TEC** | Evaluación de seguridad en desarrollos realizados por terceros. | ☐ |
| **A** | **TEC** | Ubicación del servidor en DMZ con protección WAF/IPS. | ☐ |
| **A** | **TEC** | Registro de actividad (Logging) y monitorización de accesos. | ☐ |
| **B** | **TEC** | Eliminación de usuarios por defecto y cambio de prefijos de BD. | ☐ |
| **B** | **TEC** | Plan de backups periódicos (ficheros + base de datos). | ☐ |
| **A** | **TEC** | Realización de auditorías o escaneos de vulnerabilidades externos. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---

