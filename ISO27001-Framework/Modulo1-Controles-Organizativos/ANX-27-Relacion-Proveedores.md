# ANX-27: Relación con Proveedores

## 🎯 Objetivo
Garantizar que la información de **Inespasa** permanezca protegida cuando terceros acceden a ella, asegurando que todos los productos y servicios contratados cumplen con nuestros estándares de ciberseguridad antes, durante y después de la relación contractual.

---

## 📋 Requisitos de Seguridad y Contratación
No basta con un contrato genérico; los acuerdos con proveedores deben ser específicos en materia de seguridad:

* **Clasificación del Acceso:** Definir exactamente a qué información acceden, quién accede y bajo qué método.
* **Cláusulas de Ciberseguridad:** Inclusión de requisitos legales (RGPD, LSSI), derechos de auditoría y penalizaciones económicas por incumplimiento o inactividad.
* **Certificaciones Exigidas:** Como medida de garantía mínima, se priorizarán proveedores certificados en **ISO 27001** (Seguridad) e **ISO 22301** (Continuidad).

---

## 🤝 Acuerdos de Nivel de Servicio (ANS / SLA)
Para los servicios tecnológicos, es crítico monitorizar el rendimiento mediante ANS detallados que incluyan:
* **Disponibilidad y Tiempos:** Horarios de servicio, tiempos de respuesta ante incidencias y procesos de escalado.
* **Gestión de Incidentes:** Protocolo de notificación obligatoria ante cualquier brecha de seguridad que afecte a Inespasa.
* **Tasa de Error:** Niveles de error permitidos y métricas de satisfacción.



---

## 🛡️ Controles de Seguridad Obligatorios
Inespasa establece controles estrictos para la cadena de suministro:
1. **Control de Acceso:** Revisión periódica de los permisos concedidos a técnicos externos.
2. **Auditoría:** Derecho de realizar controles y revisiones técnicas sobre los servicios prestados.
3. **Gestión de la Cadena de Suministro:** Extender estas prácticas a los subcontratistas del proveedor para evitar "puntos ciegos".

---

## 🏁 Finalización del Servicio (Offboarding)
Al terminar una relación contractual, se deben ejecutar acciones de limpieza obligatorias:
* **Revocación inmediata:** Eliminación de todos los permisos de acceso lógico (VPN, cuentas, etc.) y físico.
* **Devolución de Activos:** Retorno de cualquier equipo o documentación propiedad de Inespasa.
* **Borrado Seguro:** Certificación del borrado de información sensible de Inespasa en los sistemas del proveedor.

---

## 📊 Matriz de Control de Proveedores

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Definición de requisitos mínimos de seguridad para proveedores. | [ ] |
| **A** | **PRO** | Elaboración de cláusulas contractuales específicas de ciberseguridad. | [ ] |
| **B** | **PRO** | Delimitación de responsabilidades legales por ambas partes. | [ ] |
| **B** | **PRO** | Establecimiento y seguimiento de los ANS (SLA) técnicos. | [ ] |
| **B** | **PRO** | Verificación de certificaciones ISO 27001 / 22301 del proveedor. | [ ] |
| **B** | **PRO** | Auditoría y control periódico de los servicios contratados. | [ ] |
| **B** | **PRO** | Procedimiento de baja y borrado de datos al finalizar contratos. | [ ] |

---
> [!IMPORTANT]
> **Nota para el Administrador:** Especial atención a los proveedores de servicios Cloud y mantenimiento IT. Su acceso debe estar limitado por el principio de "mínimo privilegio" y ser siempre auditable mediante logs.
