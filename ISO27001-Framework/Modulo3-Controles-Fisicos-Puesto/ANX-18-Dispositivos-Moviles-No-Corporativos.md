# Anexo 18: Política de Dispositivos Personales (BYOD)

## 🎯 Objetivo
Establecer las directrices de seguridad para el uso de dispositivos propiedad del empleado (Smartphones, Tablets, Laptops) en el ámbito corporativo, garantizando que el acceso a la información de la organización no comprometa la integridad de la red interna.

---

## 🛠️ Normativa y Procedimientos BYOD

### 1. Requisitos de Acceso
* **Autorización Previa:** Solo los dispositivos registrados y autorizados por el departamento de IT podrán acceder a los recursos corporativos.
* **Integridad del Terminal:** Queda estrictamente prohibido el uso de dispositivos con el sistema operativo manipulado (**Root** en Android o **Jailbreak** en iOS), debido a la vulnerabilidad que suponen al permitir software de repositorios no oficiales.
* **Estado del Dispositivo:** Es obligatorio mantener el sistema operativo y las aplicaciones de seguridad actualizadas a la última versión disponible.

### 2. Gestión de Aplicaciones y Datos
* **Lista de Aplicaciones Prohibidas:** La organización mantendrá una lista negra de aplicaciones (Apps que solicitan permisos excesivos de geolocalización, acceso a contactos o lectura de archivos) que no podrán convivir en el dispositivo con las herramientas corporativas.
* **Control de Almacenamiento:** * Se permite la consulta de información en plataformas Cloud corporativas.
    * Se restringe la edición o descarga de documentos críticos en el almacenamiento local del dispositivo personal.
* **Desvinculación:** Se establece un protocolo de borrado de datos corporativos (Wipe selectivo) para cuando el empleado cese su relación con la organización o cambie de terminal.

---

## 🌐 Conectividad y Acceso Seguro

### 1. Control de Redes
* **Redes Inalámbricas:** Se prohíbe el uso de redes Wi-Fi públicas o desconocidas para el acceso a datos de la empresa. En movilidad, se priorizará el uso de la conexión de datos móviles (4G/5G).
* **Autenticación:** El acceso a la red se realizará mediante **VPN con cifrado de extremo a extremo** y sistemas de **Doble Factor de Autenticación (MFA)**.



### 2. Visibilidad y Registro
IT mantendrá un registro actualizado que incluya:
* Usuario responsable.
* Identificación técnica del dispositivo.
* Niveles de acceso y privilegios asignados.

---

## ⚠️ Gestión de Pérdida o Extravío

Ante la pérdida de un dispositivo vinculado a la red corporativa, se activarán las siguientes medidas de emergencia:
1.  **Bloqueo Remoto:** Ejecución inmediata de bloqueo de pantalla.
2.  **Borrado Remoto:** Eliminación de las cuentas y datos corporativos configurados en el terminal.
3.  **Localización:** Uso de servicios de geolocalización (si están autorizados) para el rastreo del activo.
4.  **Revocación:** Cambio inmediato de todas las credenciales del usuario afectado.



---

## ✅ Checklist de Control

| Nivel | Alcance | Control | Estado |
| :--- | :--- | :--- | :---: |
| **B** | **PRO** | Existencia de normativa BYOD firmada por el usuario. | ☐ |
| **B** | **PRO** | Plan de formación y concienciación en seguridad móvil. | ☐ |
| **B** | **TEC** | Registro de dispositivos y control de "Jailbreak/Root". | ☐ |
| **A** | **TEC** | Implementación de VPN y MFA para acceso remoto. | ☐ |
| **B** | **TEC** | Capacidad de borrado remoto de datos corporativos. | ☐ |
| **B** | **PER** | Desactivación de Bluetooth/Wi-Fi en entornos no seguros. | ☐ |
| **B** | **PER** | Uso obligatorio de bloqueo de pantalla (PIN/Biometría). | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---

