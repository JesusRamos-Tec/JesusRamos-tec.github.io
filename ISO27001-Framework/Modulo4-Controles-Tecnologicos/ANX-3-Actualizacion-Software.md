# Anexo 3: Política de Actualización de Software y Gestión de Parches

## 🎯 Objetivo
Establecer un proceso sistemático para la identificación, prueba e instalación de actualizaciones y parches de seguridad. El fin es mitigar vulnerabilidades y asegurar la estabilidad operativa de todos los activos de software de la organización.

---

## 🛠️ Ciclo de Gestión de Actualizaciones

### 1. Identificación y Alertas
La organización mantendrá un sistema de vigilancia activa para recibir notificaciones sobre nuevas vulnerabilidades (CVE) y parches:
* **Suscripciones:** Boletines de seguridad de fabricantes (Microsoft, Adobe, etc.) y organismos de ciberseguridad (INCIBE, CCN-CERT).
* **Herramientas de Diagnóstico:** Uso de escáneres de vulnerabilidades para detectar software desfasado en la red.

### 2. Evaluación y Planificación
Antes de cada despliegue, el departamento de IT determinará:
* **Criticidad:** Prioridad de la actualización (Inmediata para parches de seguridad críticos vs. Programada para mejoras funcionales).
* **Impacto:** Análisis de posibles interferencias con las operaciones de negocio. Se establecerán ventanas de mantenimiento fuera del horario crítico.

### 3. Entorno de Pruebas (Staging) y Rollback
* **Validación:** Las actualizaciones "Avanzadas" se probarán primero en un entorno aislado o en un grupo de equipos piloto para verificar la compatibilidad.
* **Plan de Marcha Atrás (Rollback):** Antes de cualquier actualización crítica, es obligatorio verificar la existencia de una copia de seguridad reciente o un punto de restauración/snapshot para poder revertir los cambios ante fallos inesperados.



---

## 📋 Registro y Auditoría
Toda actualización relevante quedará documentada en el **Registro de Cambios**, detallando:
* Fecha de instalación.
* Software y versión aplicada.
* Equipos o sistemas afectados.
* Resultado de la operación y posibles incidencias.

---

## ✅ Checklist de Control

| Nivel | Alcance | Control | Estado |
| :--- | :--- | :--- | :---: |
| **B** | **PRO** | Inventario de software corporativo sujeto a actualizaciones. | ☐ |
| **B** | **TEC** | Revisión de requisitos y características antes del despliegue. | ☐ |
| **A** | **TEC** | Validación previa en entorno de pruebas (Staging). | ☐ |
| **A** | **TEC** | Definición de procedimientos de Rollback y restauración. | ☐ |
| **A** | **TEC** | Uso de herramientas de autodiagnóstico de vulnerabilidades. | ☐ |
| **B** | **TEC** | Configuración de alertas de seguridad y boletines técnicos. | ☐ |
| **B** | **TEC** | Mantenimiento del Registro Histórico de Actualizaciones. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________
