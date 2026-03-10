# Proyecto: Reingeniería de Infraestructura de Red y Segmentación Lógica

## 🎯 Objeto del Proyecto
Este proyecto define el replanteo integral de la topología de red para garantizar la alta disponibilidad, la integridad de los datos y la seguridad perimetral. Se basa en una arquitectura jerárquica con segmentación por VLANs y optimización del direccionamiento mediante máscaras de longitud variable (VLSM).

---

## 🌐 Diseño de la Topología Lógica

### Segmentación por VLANs
Para mitigar dominios de difusión y aumentar la seguridad interna, se establece la siguiente estructura de red (Rango Base: `10.10.0.0/16`):

| ID VLAN | Nombre | Propósito | Rango IP Sugerido |
| :--- | :--- | :--- | :--- |
| **VLAN 10** | MGMT-CORE | Gestión de switches, routers y FW | 10.10.10.0/24 |
| **VLAN 20** | SERVERS | Servidores críticos y almacenamiento | 10.10.20.0/24 |
| **VLAN 30** | CORP-DATA | Usuarios de oficina y administración | 10.10.30.0/24 |
| **VLAN 40** | PRODUCTION | Terminales de planta y maquinaria | 10.10.40.0/24 |
| **VLAN 50** | IOT-PRINT | Impresoras, etiquetadoras y sensores | 10.10.50.0/24 |
| **VLAN 60** | CCTV | Cámaras de seguridad y videovigilancia | 10.10.60.0/24 |
| **VLAN 90** | GUEST-WIFI | Acceso restringido para visitas | 10.10.90.0/24 |

---

## 🛠️ Plan de Subnetting (Optimización VLSM)
Para maximizar el uso del espacio de direcciones, se propone una división en subredes que permita escalabilidad hasta 32 subredes con un total de 126 hosts por segmento (Máscara /25), adaptándose a las necesidades de cada área técnica:

* **Subredes Críticas (Gestión y Control):** Segmentos aislados para infraestructura de red.
* **Subredes de Operaciones:** Segmentos de alta densidad para terminales de usuario y dispositivos de captura de datos.

---

## 🏗️ Topología Física de Alta Disponibilidad
La infraestructura se distribuye en una arquitectura de **Estrella Extendida** mediante enlaces de fibra óptica (FTTH/SM) entre los centros de datos (CPD):

1.  **Core Layer:** Implementación de Firewall de nueva generación (NGFW) para inspección de tráfico entre VLANs y filtrado perimetral.
2.  **Distribution Layer:** Switches gestionables con capacidades L3 para enrutamiento inter-VLAN.
3.  **Access Layer:** Switches de acceso con seguridad de puerto (Port-Security) para terminales finales.

---

## 🔒 Medidas de Seguridad Implementadas
* **Aislamiento de Tráfico:** El tráfico de cámaras (CCTV) y producción no tiene visibilidad sobre la red de gestión.
* **Control de Acceso:** Implementación de listas de control de acceso (ACLs) en el firewall perimetral.
* **Resiliencia:** Conectividad redundante entre naves para asegurar la continuidad del negocio ante fallos de enlace.
