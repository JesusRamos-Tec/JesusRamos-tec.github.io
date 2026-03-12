# ANX-09: Almacenamiento en Equipo Local

## 🎯 Objetivo
Establecer las reglas, criterios y procedimientos para el mantenimiento seguro de la información almacenada localmente en los equipos corporativos, garantizando su integridad y facilitando su migración a entornos centralizados.

---

## 🛠️ Directrices de Almacenamiento

### 1. Uso y Ubicación de la Información
* **Información Autorizada:** Los empleados solo podrán almacenar información que haya sido aprobada previamente por la organización.
* **Estructura de Directorios:** Se debe seguir la normativa específica que detalla en qué nodos del árbol de directorios se debe guardar la información de trabajo, facilitando así futuras migraciones a servidores.

### 2. Ciclo de Vida del Dato Local
Para optimizar el rendimiento y la seguridad del almacenamiento local, se establecen los siguientes periodos:
* **Conservación Local:** Se define un tiempo máximo de permanencia de la información en discos locales. Una vez transcurrido, se decidirá su transferencia a servidores corporativos o su eliminación definitiva.
* **Permanencia Post-Migración:** Tras transferir los datos a servidores centrales, se establece un periodo de permanencia residual en local para evitar duplicidades antes de su borrado definitivo del disco duro.

### 3. Medidas de Seguridad Técnica
* **Cifrado Obligatorio:** Toda documentación crítica o sensible debe ser cifrada antes de su almacenamiento local, siguiendo la *Política de uso de técnicas criptográficas* para mitigar riesgos de fuga o acceso no autorizado.
* **Cumplimiento:** Es responsabilidad del empleado conocer y aplicar estas directrices, así como las políticas de seguridad relacionadas.

---

## 📊 Matriz de Control de Almacenamiento Local

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Regulación del tipo de información permitida en equipos corporativos. | ☐ |
| **B** | **PRO** | Instrucción a empleados sobre la ruta oficial de guardado de archivos. | ☐ |
| **B** | **PRO** | Definición de tiempos de conservación antes de migración o eliminación. | ☐ |
| **A** | **PRO/TEC** | Control de permanencia de datos duplicados tras la migración al servidor. | ☐ |
| **A** | **TEC/PER** | Aplicación de cifrado en información crítica almacenada localmente. | ☐ |
| **B** | **PER** | Verificación del conocimiento y aplicación de la normativa por el personal. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---

> [!NOTE]
> La correcta aplicación de este anexo reduce drásticamente el impacto de un fallo de hardware local, al asegurar que la información relevante sea movida a sistemas con alta disponibilidad y respaldo.
