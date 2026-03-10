# ANX-21: Respuesta a Incidentes de Seguridad

## 🎯 Objetivo
Garantizar que la organización cuenta con un procedimiento rápido, eficaz y documentado para actuar ante cualquier incidente de seguridad, minimizando el impacto y evitando su repetición en el futuro.

---

## 👥 Equipo Responsable
La gestión de incidentes no es solo una tarea técnica; requiere coordinación en dos niveles:
* **Personal Técnico:** Encargados de la contención, resolución y análisis forense (pueden ser internos o soporte externo).
* **Dirección:** Personal responsable de la toma de decisiones estratégicas y de estar informado sobre el estado crítico del incidente.

---

## 🛠️ Procedimiento de Actuación

### 1. Detección y Evaluación
Identificación de situaciones anómalas y categorización según su tipología y criticidad (Baja, Media, Alta, Crítica).

### 2. Resolución y Contención
Para cada tipo de incidente (malware, acceso no autorizado, fuga de datos, etc.), se seguirán acciones específicas:
* **Recogida de Evidencias:** Captura de pruebas inmediatamente después del incidente, garantizando la **cadena de custodia** y la integridad de los datos.
* **Contención:** Ejecución de medidas para reparar o mitigar los daños (aislamiento de redes, apagado de servidores, etc.).
* **Análisis Forense:** Estudio profundo del origen del ataque cuando sea preciso.
* **Escalado:** Protocolo de aviso a niveles superiores si el incidente supera la capacidad de resolución técnica inicial.

### 3. Registro del Incidente
Cada evento debe quedar documentado con la siguiente información mínima:
* Fecha y hora (inicio y resolución).
* Gravedad y recursos afectados.
* Acciones ejecutadas y personal involucrado.
* Estado actual y cierre oficial.

---

## ⚖️ Cumplimiento Legal (RGPD)
En caso de que el incidente suponga una **brecha de seguridad de datos personales**, se activará el protocolo de notificación a la Agencia Española de Protección de Datos (AEPD) y a los interesados según los plazos legales establecidos.

---

## 📊 Matriz de Control de Incidentes

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Designación del equipo responsable de gestión de incidentes. | [ ] |
| **B** | **PRO** | Proceso de Mejora Continua basado en lecciones aprendidas. | [ ] |
| **B** | **PRO** | Revisión periódica del plan de gestión (Caducidad: __________). | [ ] |
| **B** | **TEC** | Definición de criterios para la detección y evaluación de incidentes. | [ ] |
| **B** | **TEC** | Protocolo de notificación interna y externa. | [ ] |
| **A** | **TEC** | Procedimientos detallados de resolución por tipología de incidente. | [ ] |
| **B** | **TEC** | Registro sistemático de toda la gestión del incidente. | [ ] |
| **B** | **PRO** | Cumplimiento del RGPD en notificaciones de brechas de privacidad. | [ ] |

---
> [!TIP]
> **Lecciones Aprendidas:** Un incidente no termina cuando se soluciona el problema técnico. Termina cuando se analiza la causa raíz y se aplica un cambio en el sistema para que no vuelva a ocurrir.
