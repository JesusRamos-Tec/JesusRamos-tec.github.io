# ANX-11: Almacenamiento en Dispositivos Extraíbles

## 🎯 Objetivo
Establecer normas de uso para los dispositivos extraíbles que garanticen la seguridad de la información corporativa y la integridad de los sistemas a los que se conectan.

---

## 📋 Normativa y Procedimientos
Para un control efectivo, la organización debe regular el uso de estos soportes mediante:

* **Registro de Dispositivos:** Mantener un inventario de los medios extraíbles autorizados por el departamento IT.
* **Condiciones de Uso:** Definir casos específicos y autorizaciones necesarias para su utilización.
* **Configuraciones de Seguridad:** Establecer los parámetros técnicos mínimos para permitir la conexión de un dispositivo a la red.
* **Cifrado Obligatorio:** Garantizar que toda información sensible almacenada en estos medios esté protegida criptográficamente.

---

## 🔄 Alternativas al Almacenamiento Físico
Para reducir el riesgo de pérdida de datos o infección por malware, se fomentarán las siguientes alternativas:
1. **Repositorios Comunes:** Uso de servidores de archivos internos para el intercambio de información.
2. **Acceso Remoto:** Implementación de VPN o entornos virtuales para trabajar desde el exterior sin necesidad de exportar datos.
3. **Cloud Corporativo:** Uso de servicios de almacenamiento en la nube autorizados y gestionados por la organización.

---

## 🛠️ Medidas Técnicas de Protección

### En el Dispositivo Extraíble
* **Cifrado de datos:** Aplicar cifrado a nivel de volumen o de archivo.
* **Autenticación:** Requerir credenciales para acceder al contenido del soporte.

### En los Equipos Locales
* **Bloqueo USB:** Deshabilitar puertos o restringir el acceso solo a dispositivos autorizados por ID.
* **Deshabilitar Autoarranque:** Evitar la ejecución automática de scripts o software malicioso al conectar un USB.
* **Cifrado de Documentos:** Medidas de protección sobre los propios archivos transferidos.

---

## 📊 Matriz de Control de Almacenamiento Extraíble

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Elaboración de la normativa de almacenamiento en dispositivos extraíbles. | [ ] |
| **B** | **PRO** | Plan de concienciación de empleados sobre riesgos de medios físicos. | [ ] |
| **B** | **PRO/TEC** | Implementación de alternativas (Clouds autorizados, repositorios comunes). | [ ] |
| **B** | **TEC** | Registro actualizado de usuarios, dispositivos y privilegios de acceso. | [ ] |
| **B** | **TEC** | Medidas técnicas de cifrado y autenticación en el propio dispositivo. | [ ] |
| **B** | **TEC** | Bloqueo de dispositivos no autorizados y deshabilitación de autoarranque (Autorun). | [ ] |
| **B** | **TEC** | Cifrado y control de acceso sobre los documentos transferidos. | [ ] |
| **B** | **PER** | Conocimiento y aceptación formal de la normativa por parte del personal. | [ ] |

---
> [!NOTE]
> **Nota del Administrador:** La concienciación es el control más barato y efectivo. Un empleado que entiende que un USB encontrado en el parking es un riesgo potencial, es la mejor barrera contra el malware.
