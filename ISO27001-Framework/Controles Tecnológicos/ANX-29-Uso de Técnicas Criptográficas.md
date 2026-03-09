# ANX-09: Uso de técnicas criptográficas
## 🎯 Objetivo
Garantizar el uso adecuado y eficaz de las técnicas criptográficas para asegurar la **Confidencialidad, Integridad, Autenticidad y el No Repudio** de la información sensible manejada por la organización, tanto en estado de reposo (almacenada) como en tránsito.

---

## 🔍 Puntos de Control y Directrices

### 1. Identificación de Información Susceptible de Cifrado
Basado en la clasificación de activos, se establece la obligatoriedad de cifrado para:
* Información sensible, de carácter personal o confidencial.
* Registros con credenciales de autenticación.
* Información almacenada en dispositivos personales o servicios Cloud de terceros.
* Información transferida a través de redes no confiables o soportes físicos no protegidos.

### 2. Firma Electrónica y Certificados Digitales
Se implementa el uso de firma electrónica para garantizar la autenticidad en trámites administrativos y comerciales:
* **Tipos de certificados:** Persona jurídica, pertenencia a empresa, representante y factura electrónica.
* **Gestión de ciclo de vida:** Supervisión de periodos de validez, gestión de almacenamiento seguro y capacidad de revocación inmediata.

### 3. Seguridad en Servicios y Comunicaciones
* **Certificados Web (SSL/TLS):** Implementación obligatoria en sitios corporativos.
* **Servicios Externos y Desarrollo:** Cláusulas de cifrado obligatorio en la contratación de servicios externos y en el desarrollo de aplicaciones (especialmente para el login de usuarios).
* **Acceso Remoto:** Uso exclusivo de túneles **VPN cifrados** para cualquier acceso desde el exterior.

### 4. Estándares Tecnológicos (Hardening)
* **Algoritmos Autorizados:** Uso prioritario de algoritmos de especificación pública y asimétricos.
* **Protocolos Seguros:**
    * **Administración:** SSH v2 (prohibido Telnet).
    * **Transferencia:** SFTP / FTPS.
    * **Web:** HTTPS para servicios críticos.
* **Redes Inalámbricas:** Configuración mínima **WPA2** (o superior).

---

## 📊 Matriz de Control de Auditoría

Para la evaluación del cumplimiento, los controles se clasifican por su **Nivel** (Básico/Avanzado) y su **Alcance** (Procesos, Tecnologías, Personas).

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Identificación de información susceptible de ser cifrada. | [ ] |
| **B** | **PRO/TEC** | Implantación de firma electrónica para e-Administración. | [ ] |
| **B** | **PRO/TEC** | Adquisición y mantenimiento de certificados web (SSL/TLS). | [ ] |
| **B** | **PRO/TEC** | Verificación de canales cifrados en servicios externos. | [ ] |
| **B** | **PRO/TEC** | Cifrado de credenciales en desarrollo de aplicaciones. | [ ] |
| **B** | **PRO/TEC** | Autorización de acceso exterior mediante canales VPN. | [ ] |
| **B** | **TEC** | Aplicación y revisión periódica de algoritmos autorizados. | [ ] |
| **B** | **TEC** | Inventariado de aplicaciones autorizadas para cifrado. | [ ] |
| **B** | **TEC** | Implementación de protocolos seguros (SSH, SFTP, HTTPS). | [ ] |
| **B** | **TEC** | Configuración de red inalámbrica con estándar de seguridad. | [ ] |

---

## 📋 Gestión de Aplicaciones Autorizadas
Se mantiene un listado de aplicaciones validadas por el departamento de IT para las siguientes funciones:
1.  Cifrado de disco de arranque.
2.  Cifrado de soportes extraíbles (USB/Discos).
3.  Cifrado de backups y bases de datos.
4.  Cifrado de correo electrónico y directorios.

---
> **Evaluación de Riesgos:** El incumplimiento de estas directrices criptográficas supone un riesgo crítico de pérdida de confidencialidad y posibles sanciones legales en materia de protección de datos.
