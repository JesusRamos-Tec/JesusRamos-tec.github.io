# ANX-07: Sistema de Copias de Seguridad (Backup)

## 🎯 Objetivo
Garantizar la disponibilidad e integridad de la información crítica mediante procedimientos de respaldo eficaces que aseguren la continuidad del negocio ante incidentes o desastres.

---

## 🛠️ Estrategia de Respaldo y Recuperación

### 1. Clasificación y Periodicidad
Se establece un inventario de activos para identificar la información crítica. La frecuencia de las copias se define según:
* **Variación de datos:** Volumen de información generada diariamente.
* **Coste y Capacidad:** Optimización del almacenamiento disponible.
* **Obligaciones Legales:** Cumplimiento con normativas de retención de datos.

### 2. Tipología de Copias
Se emplearán, según la necesidad técnica, los siguientes métodos:
* **Completa:** Backup total de los datos seleccionados.
* **Incremental:** Solo datos modificados desde la última copia (cualquier tipo).
* **Diferencial:** Solo datos modificados desde la última copia completa.

### 3. Gestión de Soportes y Ubicación
* **Seguridad Física:** Al menos una copia completa debe residir fuera de las instalaciones de la organización.
* **Custodia:** Queda prohibido el almacenamiento de backups con datos personales en domicilios particulares. Se valorarán servicios de guardia y custodia externos.
* **Ciclo de Vida:** Los soportes deben etiquetarse individualmente y, al finalizar su vida útil, ser destruidos de forma segura para evitar recuperaciones malintencionadas.

---

## 🔐 Medidas de Protección Técnica
* **Cifrado:** Obligatoriedad de cifrar toda copia que contenga información confidencial o que sea subida a servicios Cloud.
* **Integridad:** Realización de pruebas de restauración anuales (o tras cambios significativos) para verificar que los datos son recuperables.
* **Sincronización Cloud:** En caso de usar la nube, se requiere un Acuerdo de Nivel de Servicio (ANS) firmado y canales de transmisión cifrados.

---

## 📊 Matriz de Control de Backups

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Mantenimiento del inventario de activos críticos para el negocio. | [ ] |
| **B** | **PRO** | Control estricto de acceso a los repositorios de backup. | [ ] |
| **B** | **PRO/TEC** | Definición de periodicidad y tipo de copia (Completa/Inc/Dif). | [ ] |
| **A** | **PRO/TEC** | Almacenamiento externo y uso de cajas ignífugas bajo llave. | [ ] |
| **B** | **PRO/TEC** | Procedimientos documentados de copia y restauración. | [ ] |
| **B** | **TEC** | Verificación periódica de la fiabilidad de la restauración. | [ ] |
| **B** | **TEC** | Registro y etiquetado de soportes físicos. | [ ] |
| **B** | **TEC** | Destrucción segura de soportes desechados. | [ ] |
| **B** | **PER/TEC** | Cifrado de backups confidenciales y copias en la nube. | [ ] |

---
> [!IMPORTANT]
> **Regla de Oro:** Un backup que no ha sido probado en una restauración exitosa no se considera un backup válido para la ISO 27001.
