# Anexo 04: Acceso desde Redes no Corporativas

## 🎯 Objetivo
Garantizar la seguridad de los activos y las comunicaciones de **Inespasa** cuando el acceso se realiza desde redes externas (domésticas, públicas o móviles), mitigando los riesgos de interceptación o intrusión.

---

## 🔐 Conexiones Seguras (VPN)
La piedra angular del acceso remoto es la Red Privada Virtual (VPN). Se deben seguir estas directrices técnicas:

* **Configuración Estricta:** Uso exclusivo de software autorizado por el departamento IT.
* **Control de Sesión:** Desconexión automática por inactividad para evitar sesiones abiertas en equipos desatendidos.
* **Permisos Personalizados:** Acceso segmentado según el perfil del usuario, nunca acceso total por defecto.



---

## 📡 Seguridad en Redes Inalámbricas y Móviles

### Wi-Fi Doméstica y Ajena
Se exige a los usuarios que sigan estas pautas de endurecimiento (*hardening*) en sus redes personales:
* **Protocolos:** Uso obligatorio de **WPA2** o superior.
* **Identidad:** Cambio del nombre de red (SSID) y de las credenciales de administración por defecto del router.
* **Redes Públicas:** Si la red no es segura, se limitará la navegación a sitios con cifrado **HTTPS** y se evitará el login en servicios críticos.

### Dispositivos Móviles
* **Conectividad bajo demanda:** Activar Wi-Fi, Bluetooth y GPS solo cuando sea necesario.
* **Higiene Digital:** Mantener el sistema operativo y las aplicaciones siempre actualizados.

---

## 💻 Uso de Equipos no Corporativos (BYOD)
Si se autoriza el uso de ordenadores personales, el usuario asume la responsabilidad de:
1. Mantener un **antivirus** y **firewall** activos y actualizados.
2. Utilizar una cuenta de usuario exclusiva y no compartida con familiares.
3. No instalar software de origen desconocido o sin licencia legal.

---

## 📊 Matriz de Control de Acceso Externo

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO/TEC** | Elaboración de la normativa para conexiones externas. | ☐ |
| **A** | **TEC** | Configuración de VPN con MFA y timeout de inactividad. | ☐ |
| **B** | **PER** | Formación en el uso correcto y situaciones de uso de la VPN. | ☐ |
| **B** | **PER** | Verificación de protocolos seguros (WPA2/HTTPS) en redes ajenas. | ☐ |
| **A** | **PER** | Auditoría de configuración segura en Wi-Fi domésticas (SSID/Pass). | ☐ |
| **B** | **PER** | Gestión selectiva de antenas (BT/Wi-Fi) en dispositivos móviles. | ☐ |
| **B** | **PER** | Cumplimiento de políticas BYOD (Equipos personales). | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---

> [!WARNING]
> **Aviso de IT:** El uso de redes Wi-Fi abiertas sin VPN corporativa queda terminantemente prohibido para el acceso a servidores internos o manejo de datos de clientes.
