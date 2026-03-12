# Anexo 05: Teletrabajo

## 🎯 Objetivo
Garantizar la seguridad de la información y los recursos corporativos de **Inespasa** durante el trabajo remoto, concienciando al personal sobre los riesgos y aplicando medidas técnicas que aseguren la confidencialidad e integridad de los datos fuera de la oficina.

---

## 📋 Gestión y Autorización
El teletrabajo no es una práctica informal, sino un proceso regulado por el departamento de IT y la dirección:

* **Normativa Específica:** Marco de reglas sobre dispositivos permitidos, sistemas y aplicaciones autorizadas.
* **Control de Usuarios:** Registro actualizado de empleados con perfil apto para el trabajo remoto.
* **Acuerdo de Teletrabajo:** Documento firmado por el empleado que detalla la duración, dispositivos facilitados y compromisos de seguridad.

---

## 🛠️ Controles Técnicos de Seguridad
Para mitigar los riesgos de trabajar en redes externas, se aplican los siguientes controles:

* **Acceso Seguro (MFA):** Uso obligatorio de contraseñas robustas y **Doble Factor de Autenticación (2FA/MFA)** siempre que sea posible.
* **Conectividad VPN:** Todo acceso a recursos internos debe realizarse mediante una **VPN extremo a extremo** cifrada. El uso de escritorio remoto (RDP) queda prohibido fuera de la VPN.
* **Cifrado de Datos:** Almacenamiento cifrado en todos los equipos (BitLocker o similar) para proteger la información ante pérdida o robo del dispositivo.
* **Virtualización:** Evaluación del uso de entornos virtuales (VDI) para aislar el trabajo del hardware físico del empleado.

---

## 💻 Dispositivos y Almacenamiento
Priorizamos el control sobre el hardware para asegurar el cumplimiento de las políticas de Inespasa:

1. **Equipos Corporativos:** Se prioriza su uso frente al personal, ya que vienen pre-configurados con antivirus, firewall y actualizaciones gestionadas por IT.
2. **Política BYOD:** Si se usan dispositivos personales, deben ser auditados y configurados previamente por el departamento técnico.
3. **Ubicación de Datos:** Prohibición de guardar información sensible en local. Se debe usar el almacenamiento en red corporativa o nube oficial según los anexos 9, 10, 11 y 12.

---

## ⚖️ Formación y Cumplimiento Legal
* **Concienciación Previa:** Formación obligatoria en ciberseguridad antes de iniciar el teletrabajo.
* **Privacidad (LOPDGDD):** Análisis de impacto para el tratamiento de datos personales fuera de la oficina, garantizando la privacidad según la Ley Orgánica 3/2018.

---

## 📊 Matriz de Control de Teletrabajo

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Difusión de la normativa de puesto remoto y auditorías de cumplimiento. | ☐ |
| **B** | **PRO/TEC** | Registro de usuarios autorizados para teletrabajo. | ☐ |
| **B** | **PRO/PER** | Firma de acuerdos de responsabilidad y entrega de equipos. | ☐ |
| **A** | **TEC** | Configuración de VPN, MFA y cifrado de soportes. | ☐ |
| **A** | **TEC** | Gestión de privilegios mínimos y aplicaciones permitidas en remoto. | ☐ |
| **A** | **TEC** | Planificación y verificación de backups en dispositivos remotos. | ☐ |
| **B** | **PER** | Uso preferente de dispositivos corporativos y redes seguras (evitar WiFi público). | ☐ |
| **A** | **PRO** | Cumplimiento legal LOPDGDD y formación específica en privacidad. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---

> [!WARNING]
> **Regla de Oro de IT:** Ante la duda sobre la seguridad de una red WiFi doméstica o pública, utiliza siempre el punto de acceso móvil (4G/5G) de tu dispositivo corporativo.
