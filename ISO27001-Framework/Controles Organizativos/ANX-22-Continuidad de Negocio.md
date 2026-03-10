# ANX-22: Continuidad de Negocio (PCN)

## 🎯 Objetivo
Diseñar, implementar y probar un **Plan de Continuidad de Negocio (PCN)** que permita recuperar la operativa habitual de **Inespasa** en un plazo razonable tras un incidente grave, garantizando la supervivencia de la organización.

---

## 🔍 Análisis de Impacto en el Negocio (BIA)
Para que el plan sea efectivo, realizamos un estudio profundo de las implicaciones de un desastre en nuestros activos críticos:
* **Identificación de Actividades:** Determinar los procesos vitales para Inespasa.
* **Dependencias:** Analizar la relación con otros procesos, proveedores o clientes clave.
* **RTO (Recovery Time Objective):** Tiempo máximo que la empresa puede permitir que una actividad esté detenida.
* **Niveles de Recuperación:** Tiempo mínimo para restablecer el servicio a un nivel aceptable de operatividad.

---

## 🛠️ Estrategia de Continuidad y Respaldo

### Política de Copias de Seguridad
La base de la recuperación recae en una política de backup robusta:
* **Alcance y Formato:** Definición de qué datos se respaldan y en qué soporte.
* **Periodicidad:** Frecuencia de las copias según la criticidad del dato.
* **Custodia Off-site:** Almacenamiento de copias en instalaciones físicas externas seguras.
* **Pruebas de Integridad:** Verificación periódica de que los datos son recuperables y están íntegros.

### Centro de Respaldo
Evaluación de la necesidad de un centro de datos alternativo (DR Site) para alojar la infraestructura crítica en caso de fallo total del CPD principal.

---

## 📢 Gestión de Crisis y Comunicación
En caso de activar el PCN, se seguirá un flujo de responsabilidades estricto:
* **Comité de Crisis:** Designación de responsables técnicos y directivos para la toma de decisiones.
* **Canales de Comunicación:** Establecimiento de medios oficiales para informar a empleados, clientes y entidades externas.
* **Notificaciones Externas:** Política definida para avisar a autoridades o servicios de emergencia si es necesario.

---

## 📊 Matriz de Control de Continuidad

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Definición del alcance del PCN basado en activos críticos. | [ ] |
| **B** | **PRO** | Establecimiento del flujo de responsabilidades en caso de desastre. | [ ] |
| **A** | **PRO/TEC** | Elaboración detallada del Análisis de Impacto en el Negocio (BIA). | [ ] |
| **B** | **PRO** | Política de comunicación y avisos a entidades externas. | [ ] |
| **B** | **PRO** | Revisión y actualización del PCN (Caducidad: __________). | [ ] |
| **A** | **PRO/TEC** | Definición de la estrategia de continuidad y centro de respaldo. | [ ] |
| **A** | **PRO/TEC** | Documentación detallada de la respuesta ante contingencias. | [ ] |
| **A** | **PRO/TEC** | Ejecución de pruebas y simulacros periódicos del plan. | [ ] |

---
> [!IMPORTANT]
> **La regla de oro:** Un plan de continuidad que no se prueba, no es un plan; es una lista de deseos. Los simulacros periódicos son obligatorios para garantizar que el equipo sabe reaccionar bajo presión.
