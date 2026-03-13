# 🔑 Reparación de Activación: Error de Archivo Manifest.xml

Este laboratorio documenta la resolución del error donde Windows pierde la activación (mostrando el mensaje "Activar Windows") tras una actualización, debido a la corrupción o borrado del archivo `Manifest.xml`.

> [!WARNING]
> **Impacto del error:** Mientras el sistema no esté activado, se bloquean las actualizaciones de seguridad y las opciones de personalización del entorno de usuario.

---

## 🛑 Escenario del Error
Tras una actualización de Windows, el sistema deja de reconocer la licencia original, asumiendo que el software no es genuino y limitando las capacidades administrativas y de configuración.

---

## 🛠️ Procedimiento de Recuperación

Para garantizar que las directivas de grupo (GPO) no interfieran con el proceso de validación, seguiremos este flujo:

### 1. Preparación del Entorno
* **Desvincular del Dominio:** Sacar el equipo del dominio de Active Directory y pasarlo a un grupo de trabajo (Workgroup).
* **Acceso Local:** Iniciar sesión con la cuenta de **Administrador Local**.

### 2. Extracción de la Clave Digital (OA3.0)
Si el equipo tiene la licencia embebida en la placa base (BIOS/UEFI), ejecutamos el siguiente comando en el Símbolo del Sistema (CMD) con privilegios de administrador para recuperar la clave original:

```cmd
wmic path softwarelicensingservice get OA3xOriginalProductKey
```

### 3. Re-activación Manual
* Copiar el código de 25 caracteres obtenido en el paso anterior.
* **Navegar a:** Inicio > Configuración > Sistema > Activación.
* Pulsar en Cambiar la clave de producto o Activar.
* Introducir la clave de licencia y pulsar Siguiente/Aceptar.

### 4. Reincorporación al Dominio
Una vez que el sistema confirme que "Windows está activado", volvemos a unir el equipo al dominio y reiniciamos para que el usuario pueda trabajar con normalidad.

---
## 💡 Nota Técnica
El uso del comando **wmic** para obtener la **OA3xOriginalProductKey** es fundamental en entornos empresariales con portátiles y equipos de marca (OEM), ya que extrae la clave directamente del hardware, evitando tener que buscar pegatinas físicas o facturas de compra.

---

## ⬅️ Navegación
[Volver al Índice SysAdmin-Playbooks](https://jesusramos-tec.github.io/SysAdmin-Playbooks/)

---
