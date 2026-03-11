# Anexo 17: Gestión de Dispositivos Móviles Corporativos

## 🎯 Objetivo
Definir las directrices de seguridad técnica y administrativa para el uso de dispositivos móviles propiedad de la organización (portátiles, smartphones y tablets), garantizando la protección de los activos de información fuera del perímetro físico corporativo.

---

## 🏗️ Gestión y Control de Activos

### 1. Inventario y Asignación
* **Procedimiento de Entrega:** Todo dispositivo debe estar registrado en el inventario centralizado de IT antes de su entrega.
* **Registro de Usuario:** Se mantendrá un registro actualizado que vincule el Número de Serie/IMEI con el empleado responsable, el software base instalado y la fecha de asignación.
* **Compromiso de Uso:** La entrega del equipo irá asociada a la firma de un documento de aceptación de condiciones de uso.

### 2. Configuración y Mantenimiento Técnico
* **Integridad del Sistema:** Queda prohibida la instalación de software no autorizado, la modificación del hardware o la alteración de parámetros del sistema operativo (incluyendo el desbloqueo/rooting de terminales).
* **Protección de Bajo Nivel:** Es obligatorio configurar una contraseña de acceso a la BIOS/UEFI y deshabilitar el arranque desde dispositivos externos no autorizados.
* **Gestión de Localización:** En caso de activar sistemas de geolocalización por seguridad o gestión de flota, se notificará explícitamente al usuario y se gestionará bajo la normativa de privacidad vigente.

---

## 🔐 Protección de la Información y Conectividad

### 1. Seguridad de los Datos
* **Principio de Necesidad:** Solo se almacenará en el dispositivo la información estrictamente necesaria para el desempeño de las funciones.
* **Sincronización:** Se priorizará el uso de herramientas corporativas en la nube o servidores de archivos para evitar versiones duplicadas y garantizar el backup de los datos.
* **Cifrado:** Toda información clasificada como confidencial debe estar cifrada en el almacenamiento local del dispositivo (ej. BitLocker para portátiles).

### 2. Comunicaciones Seguras
* **Redes Confiables:** Se evitará el uso de redes Wi-Fi públicas o abiertas para el acceso a sistemas corporativos.
* **Acceso Remoto:** Siempre que sea posible, se utilizarán conexiones de datos móviles (4G/5G) o redes privadas conocidas. El acceso a la infraestructura interna se realizará obligatoriamente mediante **VPN con Autenticación de Doble Factor (MFA)**.

---

## 🛡️ Normativa de Custodia y Respuesta ante Incidentes

### 1. Transporte y Custodia Física
* **Protección Ambiental:** Evitar la exposición a temperaturas extremas o condiciones que degraden los componentes.
* **Vigilancia Activa:** No abandonar el equipo en vehículos, transporte público o lugares de acceso no restringido. En entornos no seguros (hoteles, ferias), el equipo debe estar anclado mediante candados de seguridad o bajo llave.

### 2. Protocolo de Emergencia
Ante la pérdida, robo o sospecha de infección por malware, el usuario debe **notificar de forma inmediata** al departamento de IT para proceder al bloqueo remoto del dispositivo y la revocación de credenciales.

---

## ✅ Checklist de Control

| Nivel | Alcance | Control | Estado |
| :--- | :--- | :--- | :---: |
| **B** | **PRO/TEC** | Procedimiento de asignación e inventariado activo. | ☐ |
| **B** | **TEC** | Registro detallado de hardware y licencias por empleado. | ☐ |
| **B** | **TEC** | Contraseña de BIOS configurada y funcional. | ☐ |
| **B** | **TEC** | Protocolo de notificación de software de localización. | ☐ |
| **B** | **PER** | Almacenamiento local restringido a lo estrictamente necesario. | ☐ |
| **B** | **PER** | Uso de conexiones cifradas o redes móviles privadas. | ☐ |
| **B** | **PER** | Cumplimiento de normas de transporte y custodia física. | ☐ |
| **B** | **PER** | Conocimiento y aceptación de responsabilidades legales. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________
