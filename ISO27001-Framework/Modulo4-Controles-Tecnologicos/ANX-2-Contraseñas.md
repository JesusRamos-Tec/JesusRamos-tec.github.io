# Anexo 02: Política de Contraseñas

## 🎯 Objetivo
Establecer, difundir y verificar el cumplimiento de las buenas prácticas en el uso de credenciales para garantizar que el acceso a los sistemas de la organización sea seguro y robusto.

---

## 🛠️ Gestión y Ciclo de Vida
Para una correcta administración de las identidades, se deben seguir estas pautas técnicas:

* **Identificación de Activos:** Determinar qué equipos, servicios y aplicaciones requieren credenciales.
* **Almacenamiento Seguro:** Las claves deben guardarse en repositorios cifrados y contar con copias de respaldo.
* **Periodos de Validez:** Establecer tiempos de expiración según la criticidad del servicio.
* **Revocación:** Procedimiento inmediato de desactivación por baja de personal o sospecha de compromiso.
* **Prohibición de Valores por Defecto:** Se debe cambiar obligatoriamente cualquier contraseña de fábrica en hardware o software.

---

## 🛡️ Robustez y Requisitos Técnicos
La organización se apoya en herramientas como **Active Directory** o **LDAP** para forzar el cumplimiento de los siguientes parámetros:

### Parámetros de Configuración
* **Longitud Mínima:** Al menos 8 caracteres.
* **Complejidad:** Combinación obligatoria de mayúsculas, minúsculas, números y símbolos.
* **Historial:** Impedir la reutilización de contraseñas anteriores.
* **Bloqueo:** Limitar el número de intentos fallidos antes de bloquear la cuenta.

### Restricciones Semánticas
Queda prohibido el uso de:
* Palabras sencillas en cualquier idioma.
* Datos personales (nombres, fechas, lugares).
* Patrones de teclado (ej: "qwerty" o "123456").

---

## 🔑 Buenas Prácticas para el Usuario
La seguridad depende directamente del comportamiento del personal:

* **Confidencialidad:** Las contraseñas son personales e intransferibles. Prohibido compartirlas o enviarlas por email/formularios no confiables.
* **No Escritura:** Prohibido anotar claves en post-its, papeles o documentos sin cifrar.
* **Unicidad:** No utilizar la misma clave para diferentes servicios.
* **Gestores de Contraseñas:** Se recomienda el uso de baúles de contraseñas autorizados en lugar de los recordatorios del navegador.

> [!CAUTION]
> **Doble Factor (MFA/2FA):** Es obligatorio para servicios críticos. Se priorizan sistemas **OTP**, tokens criptográficos o tarjetas de coordenadas. Según la directiva **EU NIS-2**, el uso de huella digital podría no ser aconsejable en ciertos contextos de alta seguridad.

---

## 📊 Matriz de Control de Contraseñas

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **A** | **PRO/TEC** | Sistema avanzado de gestión del ciclo de vida de claves. | ☐ |
| **A** | **PRO/TEC** | Uso de sistemas de autenticación externos descentralizados. | ☐ |
| **A** | **TEC** | Herramientas técnicas para forzar la seguridad (GPO/AD). | ☐ |
| **B** | **TEC** | Cambio obligatorio de contraseñas por defecto. | ☐ |
| **B** | **TEC** | Implementación de Doble Factor en servicios críticos. | ☐ |
| **B** | **PER** | Prohibición de compartir credenciales. | ☐ |
| **B** | **PER** | Creación de contraseñas siguiendo criterios de robustez. | ☐ |
| **B** | **PER** | Rotación periódica de contraseñas cada __________. | ☐ |
| **B** | **PER** | Uso de gestores de contraseñas oficiales de la empresa. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---

