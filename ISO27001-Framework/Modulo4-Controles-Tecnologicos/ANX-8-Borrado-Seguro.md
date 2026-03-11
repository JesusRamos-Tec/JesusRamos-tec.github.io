# Anexo 8: Política de Borrado Seguro y Destrucción de Soportes

## 🎯 Objetivo
Establecer los procedimientos técnicos y organizativos para asegurar que la información sensible sea eliminada de forma irreversible cuando ya no sea necesaria, evitando la recuperación no autorizada de datos desde soportes obsoletos, averiados o reutilizados.

---

## 📋 Gestión y Clasificación de Soportes

### 1. Inventario y Seguimiento de Activos
La organización mantendrá un inventario actualizado de todos los soportes de almacenamiento (discos duros, SSD, cintas de backup, memorias USB, móviles). Cada activo debe tener:
* **Responsable:** Usuario o departamento asignado.
* **Clasificación:** Nivel de criticidad de la información que contiene.
* **Historial:** Registro de mantenimientos, reparaciones y cambios de custodia.

### 2. Cadena de Custodia
Cualquier soporte que contenga información corporativa y deba ser reparado o sustituido debe seguir un control estricto de custodia. Si el soporte debe salir de las instalaciones para reparación, la información debe ser cifrada previamente (Anexo 29) o el soporte debe ser destruido si no es posible garantizar su seguridad.

---

## 🛠️ Métodos de Eliminación de Información

Dependiendo del destino del soporte, se aplicarán diferentes técnicas de borrado:

### A. Reutilización Interna (Borrado Lógico)
Para soportes que permanecerán en la organización pero cambian de usuario:
* **Sobreescritura:** Uso de software especializado que escribe patrones de datos aleatorios en toda la superficie del disco (mínimo 3 pasadas para discos magnéticos).
* **Crypto-Erase:** Para unidades con cifrado nativo, se procede al borrado seguro de las llaves criptográficas, haciendo los datos inaccesibles.

### B. Desincorporación o Desecho (Destrucción Física)
Para soportes que salen de la organización o están averiados:
* **Desmagnetización (Degaussing):** Aplicación de campos magnéticos de alta intensidad (solo para medios magnéticos).
* **Destrucción Mecánica:** Triturado, perforación o fundición del soporte para hacer físicamente imposible la recuperación de los platos o chips de memoria.
* **Dispositivos Especiales:** Se asegura el borrado de memorias volátiles y no volátiles en impresoras, fotocopiadoras, GPS y terminales móviles antes de su entrega a gestores de residuos.



---

## ✅ Certificación y Cumplimiento
* **Evidencia del Proceso:** Toda operación de borrado avanzado debe generar un certificado o informe que detalle el método usado, la fecha y el identificador del dispositivo (SN/ID).
* **Terceros Homologados:** En caso de usar empresas externas para la destrucción, estas deben emitir un **Certificado de Destrucción** que garantice el cumplimiento del RGPD y las normativas medioambientales.

---

## ✅ Checklist de Control

| Nivel | Alcance | Control | Estado |
| :--- | :--- | :--- | :---: |
| **B** | **PRO** | Mantenimiento del inventario de activos y su criticidad. | ☐ |
| **B** | **PRO/TEC** | Supervisión y documentación del ciclo de vida de los soportes. | ☐ |
| **A** | **PRO/TEC** | Destrucción de información en soportes no electrónicos (papel). | ☐ |
| **A** | **PRO/TEC** | Uso de sobreescritura certificada para la reutilización de discos. | ☐ |
| **A** | **PRO/TEC** | Destrucción física o desmagnetización antes del desecho de hardware. | ☐ |
| **A** | **PRO/TEC** | Borrado de memorias en dispositivos periféricos (impresoras/móviles). | ☐ |
| **A** | **TEC** | Emisión de informes técnicos de cada operación de borrado. | ☐ |
| **A** | **TEC** | Contratación de servicios de destrucción certificada por terceros. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________
