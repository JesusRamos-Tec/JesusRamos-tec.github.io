# ANX-09: Estándares de Criptografía y Cifrado

## 🎯 Objetivo
Garantizar la confidencialidad, integridad y autenticidad de la información mediante el uso de controles criptográficos adecuados, minimizando los riesgos de acceso no autorizado o manipulación de datos.

---

## 🛠️ Especificaciones Técnicas y Algoritmos Autorizados

Para asegurar un nivel de protección robusto, se establecen los siguientes estándares obligatorios para la organización:

### 1. Comunicaciones Inalámbricas (Wi-Fi)
- **Estándar Mínimo:** WPA2-Enterprise con cifrado AES.
- **Estándar Recomendado:** WPA3.
- **Restricción:** Queda prohibido el uso de protocolos obsoletos o vulnerables como WEP o WPA (TKIP).

### 2. Acceso Remoto y Administración de Sistemas
- **VPN (Virtual Private Network):** Uso obligatorio de túneles cifrados mediante protocolos SSL/TLS o IPsec con algoritmos de intercambio de claves seguros.
- **Protocolos de Gestión:** - Acceso a servidores vía **SSH v2** (deshabilitando v1).
  - Transferencia de archivos mediante **SFTP** o **HTTPS**.
  - RDP solo permitido a través de Gateway VPN.

### 3. Almacenamiento de Información (Data at Rest)
- **Cifrado de Puestos de Trabajo:** Uso de BitLocker (Windows) o FileVault (macOS) con cifrado mínimo de **AES-256 bits**.
- **Dispositivos Extraíbles:** Obligatoriedad de cifrado en cualquier soporte que contenga datos corporativos.

---

## ✅ Checklist de Control de Auditoría

| ID | Control de Seguridad | Cumplimiento | Observaciones |
| :--- | :--- | :---: | :--- |
| **9.1** | ¿Se utilizan algoritmos de cifrado simétrico AES-256 para datos sensibles? | [ ] | Estándar de la industria. |
| **9.2** | ¿Se han deshabilitado protocolos de comunicación no cifrados (Telnet, FTP, HTTP)? | [ ] | Reemplazados por SSH, SFTP, HTTPS. |
| **9.3** | ¿Se emplean certificados digitales vigentes (SSL/TLS) para servicios web? | [ ] | Verificación de CA autorizada. |
| **9.4** | ¿Existe una política de acceso desde el exterior basada exclusivamente en VPN? | [ ] | Auditoría de túneles activos. |
| **9.5** | ¿Las credenciales en bases de datos se almacenan con algoritmos de Hash (SHA-256 o superior)? | [ ] | Prohibido texto plano. |

---

> [!IMPORTANT]
> **Nota del Auditor:** El uso de criptografía debe revisarse anualmente para asegurar que los algoritmos empleados no han sido declarados obsoletos por la comunidad de ciberseguridad.
