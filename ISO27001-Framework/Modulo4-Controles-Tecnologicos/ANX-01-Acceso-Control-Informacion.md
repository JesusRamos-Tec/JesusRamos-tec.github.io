# Anexo 01: Acceso y Control a la Información

## 🎯 Objetivo
Determinar de manera precisa quién, cómo y cuándo se accede a los activos de información de la organización, garantizando que dichos accesos queden debidamente registrados y autorizados.

---

## 🔐 Directrices de Control de Acceso

### 1. Gestión de Grupos y Usuarios
El acceso a la información no es universal; se segmenta en función de tres criterios críticos:
* **Pertenencia:** El departamento o área específica del empleado.
* **Sensibilidad:** El tipo de información a la que se intenta acceder.
* **Operatividad:** Qué acciones tiene permitido realizar (lectura, escritura, ejecución, etc.).

> [!IMPORTANT]
> **Principio de Mínimo Privilegio:** Como norma general, solo se otorgarán los permisos estrictamente necesarios para el desempeño de la función laboral.

### 2. Cuentas de Administración (Privilegiadas)
Dada su criticidad, las cuentas de administrador requieren un control exhaustivo:
* **Cuentas específicas:** Uso de cuentas dedicadas exclusivamente a tareas de administración.
* **MFA Obligatorio:** Uso de doble factor de autenticación para mitigar riesgos de suplantación.
* **Trazabilidad:** Registro íntegro de todas las acciones realizadas bajo privilegios elevados.
* **Aislamiento:** Evitar la herencia de privilegios y asegurar que el entorno de administración sea claramente identificable durante la sesión.
* **Auditoría:** Estas cuentas están sujetas a revisiones y auditorías periódicas.

### 3. Mecanismos de Autenticación
Se implementarán sistemas basados en tres factores fundamentales:
1. **Algo que sabemos:** Contraseñas robustas y de cambio periódico.
2. **Algo que tenemos:** Dispositivos físicos o tokens (MFA).
3. **Algo que somos:** Biometría u otros factores de identidad únicos.

---

## 🔄 Ciclo de Vida de las Cuentas

### Altas, Modificaciones y Bajas
Todo cambio en las cuentas de usuario debe seguir un procedimiento formal que incluya:
* **Autorización:** Identificación clara de quién autoriza el acceso.
* **Confidencialidad:** Entrega segura y privada de las credenciales iniciales.
* **Revisiones Periódicas:** Verificación recurrente de que los permisos siguen siendo adecuados para el puesto.

### Revocación por Cese Contractual
Al finalizar la relación con la organización, se ejecutarán de inmediato las siguientes acciones:
* Revocación total de permisos de acceso físico y lógico.
* Eliminación de cuentas de correo y accesos a repositorios o aplicaciones Cloud.
* Devolución obligatoria de activos (portátiles, tarjetas de acceso, dispositivos de almacenamiento).

---

## 📊 Matriz de Control de Acceso

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Definición de roles y grupos según el tipo de información. | ☐ |
| **B** | **PRO** | Aplicación de la política de asignación de mínimos privilegios. | ☐ |
| **B** | **TEC** | Procedimiento formal de gestión de identidades (Altas/Bajas). | ☐ |
| **B** | **TEC** | Gestión específica y segura de cuentas de administración. | ☐ |
| **A** | **TEC** | Implantación de mecanismos de autenticación multifactor (MFA). | ☐ |
| **A** | **TEC** | Registro de eventos y logs de acceso a la información. | ☐ |
| **B** | **TEC** | Revisión periódica de permisos concedidos a usuarios. | ☐ |
| **B** | **TEC** | Revocación inmediata de accesos tras fin de contrato. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---

> [!TIP]
> **Registro de Eventos:** Es vital registrar no solo el "quién", sino también el "cuándo" y la "finalidad" del acceso para cumplir con los estándares de trazabilidad de la ISO 27001.
