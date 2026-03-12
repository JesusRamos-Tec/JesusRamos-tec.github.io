# Anexo 10: Almacenamiento en Red Corporativa

## 🎯 Objetivo
Establecer las directrices para el uso eficiente y seguro de los recursos de almacenamiento centralizado. El fin es garantizar la integridad de la información, evitar la duplicidad de datos, facilitar el trabajo colaborativo y asegurar la correcta ejecución de las políticas de backup.

---

## 🏗️ Directrices de Almacenamiento Centralizado

### 1. Criterios de Uso
La organización establece que la información corporativa debe residir en servidores centralizados bajo los siguientes criterios:
* **Naturaleza de la Información:** Solo se almacenará información de carácter profesional y necesaria para el desempeño de las funciones laborales.
* **Responsabilidad:** Los usuarios son responsables de la organización de sus directorios asignados y de la eliminación de información obsoleta o duplicada.
* **Propiedad:** Todos los datos almacenados en la red corporativa son propiedad de la organización y están sujetos a las políticas de auditoría y seguridad vigentes.

### 2. Clasificación y Control de Acceso
El almacenamiento se estructurará siguiendo la **Política de Clasificación de la Información**:
* **Directorios de Departamento:** Acceso restringido a los miembros del área correspondiente.
* **Directorios de Intercambio:** Espacios temporales para proyectos transversales con permisos específicos.
* **Directorios Personales:** Espacios privados para el usuario, pero respaldados por el sistema de backups centralizado.

### 3. Medidas Técnicas de Protección
* **Cuotas de Almacenamiento:** Se implementarán límites de espacio para garantizar la disponibilidad del servicio para todos los usuarios.
* **Cifrado:** Los volúmenes que contengan información crítica o datos de carácter personal deberán estar cifrados en reposo.
* **Auditoría:** El departamento de IT realizará revisiones periódicas de los registros de acceso y del estado de capacidad de los servidores.

---

## 💾 Gestión de Copias de Seguridad (Backup)
Toda información almacenada en la red corporativa está integrada en el **Plan de Continuidad de Negocio**:
* **Frecuencia:** Copias diarias (incrementales) y semanales (completas).
* **Retención:** Se definirá un periodo de conservación acorde a la sensibilidad de los datos y la normativa legal.
* **Verificación:** Pruebas periódicas de restauración para garantizar la disponibilidad de los datos ante un desastre.

---

## ✅ Checklist de Control

| Nivel | Alcance | Control | Estado |
| :--- | :--- | :--- | :---: |
| **B** | **PRO** | Inventario actualizado de servidores y recursos de red. | ☐ |
| **B** | **PRO** | Comunicación a empleados sobre criterios de almacenamiento. | ☐ |
| **B** | **PRO** | Aplicación de la Política de Clasificación de Información. | ☐ |
| **A** | **PRO/TEC** | Implementación de listas de control de acceso (ACLs). | ☐ |
| **A** | **PRO/TEC** | Ejecución y verificación del Plan de Copias de Seguridad. | ☐ |
| **A** | **TEC** | Configuración de cuotas y alertas de capacidad. | ☐ |
| **A** | **TEC** | Auditoría periódica de logs de acceso y uso de disco. | ☐ |
| **A** | **TEC/PER** | Cifrado de información crítica en servidores. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---

