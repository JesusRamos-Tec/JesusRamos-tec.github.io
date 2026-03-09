# ANX-05: Directrices de Seguridad para el Teletrabajo

## 🎯 Objetivo
Establecer las medidas de seguridad técnicas y organizativas necesarias para proteger la información y los recursos corporativos cuando se accede a ellos desde ubicaciones remotas, garantizando la continuidad del negocio y el cumplimiento legal (LOPDGDD).

---

## 📋 Marco Normativo y Operativo

### 1. Gestión de Usuarios y Autorizaciones
* **Control de Acceso:** Se mantiene una relación actualizada de usuarios autorizados para el trabajo en remoto según su perfil de riesgo.
* **Acuerdo de Teletrabajo:** Todo empleado debe firmar un documento de compromiso que detalle la duración, los dispositivos facilitados y las responsabilidades en materia de seguridad.
* **Principio de Menor Privilegio:** El acceso remoto se limita estrictamente a las aplicaciones y recursos necesarios para el desempeño de la labor diaria.

### 2. Configuración Técnica del Puesto Remoto
* **Hardening de Dispositivos:** Todos los equipos (corporativos o BYOD) deben ser configurados previamente por el departamento de IT (Antivirus, parches, firewall).
* **Cifrado Obligatorio:** Uso de cifrado de disco completo para proteger los datos ante pérdida o robo del dispositivo.
* **Almacenamiento Seguro:** Prohibición de almacenamiento local persistente; se prioriza el uso de la red corporativa y soluciones Cloud autorizadas con backup centralizado.

### 3. Conectividad y Acceso Seguro
* **Túneles VPN:** Uso obligatorio de VPN extremo a extremo para cifrar el tráfico entre el host remoto y la LAN corporativa.
* **Escritorio Remoto (RDP):** Queda prohibido el uso de RDP directo a internet; solo se permite a través de la pasarela VPN.
* **Doble Factor (MFA):** Implementación de autenticación multifactor para validar la identidad del usuario.
* **Redes Confiables:** Recomendación de uso de redes domésticas seguras o datos móviles (4G/5G). Se prohíbe el uso de Wi-Fi públicas para tráfico sensible.

---

## 📊 Matriz de Control de cumplimiento

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Normativa de protección del puesto de trabajo remoto y auditorías. | [ ] |
| **B** | **PRO/TEC** | Registro actualizado de usuarios con permisos de acceso remoto. | [ ] |
| **B** | **PRO/PER** | Procedimientos de solicitud y firma de compromiso de teletrabajo. | [ ] |
| **A** | **TEC** | Gestión de privilegios y acceso limitado a aplicaciones por perfil. | [ ] |
| **A** | **TEC** | Implementación de MFA y política de contraseñas robustas. | [ ] |
| **A** | **TEC** | Hardening y configuración de seguridad en dispositivos (EDR/AV). | [ ] |
| **A** | **TEC** | Cifrado de soportes de información (Data-at-rest). | [ ] |
| **B** | **TEC** | Definición de rutas de almacenamiento oficial (Red/Cloud). | [ ] |
| **A** | **TEC** | Planificación y verificación de restauración de backups remotos. | [ ] |
| **A** | **TEC** | Despliegue de VPN corporativa para cifrado de comunicaciones. | [ ] |
| **A** | **TEC** | Virtualización de entornos de trabajo (VDI) para mitigar riesgos. | [ ] |
| **B** | **PER** | Priorización de uso de equipamiento corporativo sobre personal. | [ ] |
| **B** | **PRO** | Plan de concienciación y formación previa al teletrabajo. | [ ] |
| **A** | **PRO** | Análisis de impacto y cumplimiento normativo LOPDGDD. | [ ] |

---

## 🎓 Concienciación del Usuario
Antes de iniciar la modalidad de teletrabajo, el personal debe recibir formación específica en:
1. Identificación de intentos de Phishing y ataques de Ingeniería Social.
2. Uso seguro de la conexión VPN.
3. Reporte inmediato de incidentes de seguridad (pérdida de dispositivos, accesos sospechosos).

---
> **Nota de Auditoría:** Este anexo debe revisarse periódicamente para adaptarse a las nuevas amenazas detectadas en entornos de trabajo híbridos.
