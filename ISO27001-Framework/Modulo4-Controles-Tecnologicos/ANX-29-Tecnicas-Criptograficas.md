# Anexo 29: Política de Uso de Técnicas Criptográficas

## 🎯 Objetivo
Garantizar la confidencialidad, integridad, autenticidad y el no repudio de la información sensible mediante el uso de mecanismos criptográficos robustos, tanto para los datos almacenados (at-rest) como para los datos en tránsito (in-motion).

---

## 🔐 Ámbito de Aplicación

### 1. Información Susceptible de Cifrado
Siguiendo la **Política de Clasificación de la Información**, se aplicará cifrado obligatoriamente a:
* **Datos Sensibles:** Información de carácter personal (RGPD), datos financieros o secretos industriales.
* **Credenciales:** Bases de datos de usuarios, archivos de configuración con contraseñas y registros de autenticación.
* **Dispositivos Móviles:** Laptops, tablets y smartphones corporativos (cifrado de disco completo).
* **Almacenamiento Externo:** Backups en la nube y soportes físicos extraíbles (pendrives, discos externos).

### 2. Algoritmos y Estándares Autorizados
La organización priorizará el uso de algoritmos de clave pública (asimétricos) y simétricos que sean de estándar abierto y ampliamente auditados:
* **Cifrado de Datos:** AES-256 o superior.
* **Protocolos de Comunicación:** TLS 1.2/1.3 para entorno web, SSH v2 para administración remota y VPN (IPsec o OpenVPN) para accesos externos.
* **Redes Inalámbricas:** Uso de WPA2-Enterprise o WPA3. Queda prohibido el uso de protocolos obsoletos como WEP o WPA.

---

## 📑 Firma Electrónica y Certificados Digitales

### 1. Uso de Firma Electrónica
Se empleará para garantizar el no repudio y la integridad en:
* Relaciones con Administraciones Públicas.
* Emisión y recepción de facturación electrónica.
* Firma de contratos y documentos oficiales de la organización.

### 2. Gestión de Certificados
El departamento de IT centralizará la gestión de certificados digitales (Persona Jurídica, Representante, etc.), supervisando:
* Periodos de validez y renovaciones automáticas.
* Almacenamiento seguro en dispositivos criptográficos (Tokens/Smartcards) o HSM.
* Procedimientos de revocación inmediata en caso de compromiso o cese de personal.

---

## 🚀 Implementación Técnica y Protocolos

### 1. Administración y Transferencia Segura
Queda estrictamente prohibido el uso de protocolos de texto plano. Se sustituirán por sus versiones seguras:
* **SSH** en lugar de Telnet/Rlogin.
* **SFTP/FTPS** en lugar de FTP.
* **HTTPS (TLS)** obligatorio para todos los servicios web corporativos.

### 2. Aplicaciones Criptográficas Autorizadas
IT mantendrá un listado de software validado para tareas de cifrado (ej. BitLocker para discos, VeraCrypt para contenedores, GPG para correo confidencial). El uso de herramientas no autorizadas se considerará una brecha de política de seguridad.

---

## ✅ Checklist de Control

| Nivel | Alcance | Control | Estado |
| :--- | :--- | :--- | :---: |
| **B** | **PRO** | Identificación de activos y flujos de datos que requieren cifrado. | ☐ |
| **B** | **PRO/TEC** | Implementación de firma electrónica en procesos legales y comerciales. | ☐ |
| **B** | **PRO/TEC** | Despliegue de certificados SSL/TLS en todos los portales web. | ☐ |
| **B** | **PRO/TEC** | Configuración de túneles VPN cifrados para accesos remotos. | ☐ |
| **B** | **TEC** | Selección y revisión de algoritmos de cifrado (AES, RSA, ECC). | ☐ |
| **B** | **TEC** | Mantenimiento del inventario de software criptográfico autorizado. | ☐ |
|
**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---

