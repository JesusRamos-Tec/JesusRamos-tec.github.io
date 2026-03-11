# Anexo 16: Clasificación de la Información

## 🎯 Objetivo
Clasificar los activos de información de la organización para garantizar una gestión de seguridad eficaz, basada en los pilares de **Confidencialidad, Integridad y Disponibilidad (CID)**.

---

## 📋 Inventario y Catalogación
Antes de proteger, debemos saber qué tenemos. El inventario de activos debe registrar:
* **Identificación:** Nombre y tipo de activo.
* **Ubicación:** Servidores, nube o soportes físicos.
* **Responsabilidad:** Propietario del activo (*Asset Owner*) y departamento al que pertenece.
* **Dimensionamiento:** Tamaño y servicios asociados.

---

## 🏷️ Criterios de Clasificación
La información se etiqueta para determinar qué medidas de seguridad aplicar:

1. **Nivel de Accesibilidad:**
   * **Confidencial:** Solo personal autorizado (ej: nóminas, estrategias).
   * **Interna:** Uso exclusivo para empleados (ej: procedimientos operativos).
   * **Pública:** Información sin restricciones (ej: catálogos comerciales).
2. **Utilidad Funcional:** Clasificación por áreas (Clientes, Compras, RRHH, Gestión Interna).
3. **Impacto por Incidente:** Evaluación de daños en caso de robo o pérdida (daño de imagen, legal, económico o paralización de la producción).

---

## 🛡️ Tratamientos de Seguridad Aplicables
Una vez clasificada la información, se aplican los controles técnicos correspondientes:

* **Control de Acceso:** Limitación estricta a grupos o personas específicas.
* **Cifrado (Encryption):** Aplicación de algoritmos de cifrado para datos confidenciales.
* **Disponibilidad:** Programación de copias de seguridad según la criticidad.
* **Cumplimiento Legal:** Medidas específicas alineadas con el **RGPD** para datos de carácter personal.
* **Confidencialidad:** Firma de acuerdos (NDA) para información sensible de terceros.

---

## 📊 Matriz de Control de Clasificación

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Elaboración del inventario detallado de activos de información. | [ ] |
| **B** | **PRO** | Definición de criterios de seguridad para la clasificación. | [ ] |
| **B** | **PRO** | Etiquetado de activos según los criterios establecidos. | [ ] |
| **B** | **PRO** | Listado de tratamientos de seguridad disponibles en la empresa. | [ ] |
| **A** | **TEC** | Aplicación técnica de tratamientos (Cifrado, ACLs, Backups). | [ ] |
| **A** | **TEC** | Realización de auditorías de comprobación periódicas (Cada: __________). | [ ] |

---
> [!TIP]
> **Visión del Administrador:** En entornos Windows, esto se traduce habitualmente en la implementación de **FSRM** (File Server Resource Manager) para clasificar archivos automáticamente o el uso de **Azure Information Protection** para etiquetar documentos en la nube.
