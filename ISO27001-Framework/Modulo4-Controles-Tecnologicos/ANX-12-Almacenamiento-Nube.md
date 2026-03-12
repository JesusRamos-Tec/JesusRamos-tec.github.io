# Anexo 12: Política de Almacenamiento en la Nube (Cloud Storage)

## 🎯 Objetivo
Definir los criterios, reglas y procedimientos para el uso seguro de servicios de almacenamiento en la nube. El objetivo es garantizar que la información corporativa mantenga sus niveles de confidencialidad, integridad y disponibilidad, independientemente de la infraestructura donde se aloje.

---

## ☁️ Gobernanza de Servicios Cloud

### 1. Autorización de Servicios
* **Uso de Cloud Pública:** Solo se permite el uso de servicios de almacenamiento en la nube pública que hayan sido previamente auditados y aprobados por el departamento de IT.
* **Lista de Servicios Permitidos (Whitelist):** La organización mantendrá un registro actualizado de plataformas autorizadas (ej. OneDrive for Business, Google Workspace, AWS S3). Queda prohibido el uso de cuentas personales o servicios no corporativos para fines profesionales ("Shadow IT").

### 2. Clasificación de Datos en la Nube
El tipo de información que puede residir en la nube se rige por la **Política de Clasificación de la Información**:
* **Información Pública/Uso Interno:** Puede almacenarse en los servicios autorizados siguiendo las configuraciones estándar.
* **Información Confidencial:** Solo podrá almacenarse en la nube si el proveedor garantiza cifrado en reposo y tránsito, y siempre que se apliquen medidas adicionales de control de acceso (MFA).

### 3. Borrado y Ciclo de Vida
Se aplicará la política de borrado seguro de la organización de forma extensiva a la nube. Cuando un proyecto finaliza o un empleado causa baja, se procederá al **Wipe selectivo** o eliminación definitiva de los repositorios en la nube para evitar la persistencia de datos residuales.

---

## 🛡️ Selección y Seguridad del Proveedor

### 1. Criterios de Contratación
Antes de la adopción de un nuevo servicio de almacenamiento cloud, se verificarán los siguientes puntos:
* **Garantías Legales:** Cumplimiento con el RGPD (Reglamento General de Protección de Datos) y leyes locales de privacidad.
* **Ubicación de los Datos:** Preferencia por centros de datos situados dentro del Espacio Económico Europeo (EEE).
* **SLA (Acuerdo de Nivel de Servicio):** Garantía de disponibilidad mínima del 99.9%.

### 2. Auditoría de Seguridad del Proveedor
Es obligatorio revisar la política de seguridad y las certificaciones (ej. ISO 27001, SOC2, esquema Nacional de Seguridad) del proveedor antes de confiarle información corporativa. Se evaluará su capacidad de respuesta ante incidentes y sus protocolos de backup.

---

## 💾 Backups y Resiliencia
Se debe evaluar la estrategia de **Backup Cloud-to-Cloud** o **Cloud-to-OnPremise**. No se debe asumir que el proveedor de la nube es el único responsable de la recuperación de los datos ante un borrado accidental o un ataque de ransomware.

---

## ✅ Checklist de Control

| Nivel | Alcance | Control | Estado |
| :--- | :--- | :--- | :---: |
| **B** | **PRO** | Comunicación oficial sobre el uso permitido/prohibido de nubes públicas. | ☐ |
| **B** | **PRO** | Publicación de la lista de servicios cloud autorizados. | ☐ |
| **B** | **PRO** | Definición del procedimiento de borrado de información en la nube. | ☐ |
| **B** | **PRO** | Formación sobre clasificación de datos aptos para entorno cloud. | ☐ |
| **A** | **PRO/TEC** | Verificación de cumplimiento legal y normativo del proveedor. | ☐ |
| **B** | **PRO/TEC** | Revisión de las certificaciones de seguridad del proveedor. | ☐ |
| **B** | **TEC** | Evaluación de riesgos antes de implementar backups en la nube. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---
