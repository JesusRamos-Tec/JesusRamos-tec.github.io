# 🐧 Lab 01: Instalación y Configuración Base de RHEL 9.7

[cite_start]Este manual documenta el proceso detallado de instalación, configuración inicial y preparación del entorno de laboratorio para la certificación **RHCSA**[cite: 1, 38].

## 🏗️ Entorno del Laboratorio
[cite_start]El despliegue se realiza sobre un nodo de virtualización **Proxmox VE 9.0.3** ejecutándose en un hardware **BMAX Pro** con 32GB de RAM y 1TB de disco duro[cite: 3].

### Especificaciones de la VM (rhca-labs)
* [cite_start]**CPU**: 1 Socket / 2 Cores (Tipo: Host para acceso real al microprocesador)[cite: 4, 30].
* [cite_start]**RAM**: 4GB (4096MB)[cite: 4, 31].
* [cite_start]**Disco**: 40GB (VirtIO)[cite: 4, 28].
* [cite_start]**Sistema**: Qemu Agent habilitado para gestión desde el hipervisor[cite: 27].

---

## 💾 Gestión de Almacenamiento (LVM)
[cite_start]Se aplica un particionado manual basado en **Logical Volume Management (LVM)** para garantizar flexibilidad en la gestión de volúmenes[cite: 5, 56, 57].

| Punto de Montaje | Tamaño | Tipo / Volume Group | Sistema de Archivos |
| :--- | :--- | :--- | :--- |
| `/boot` | [cite_start]1024 MiB [cite: 6, 59] | [cite_start]Partición Estándar [cite: 6, 59] | [cite_start]XFS [cite: 8] |
| `swap` | [cite_start]2 GiB [cite: 9, 60] | [cite_start]LV en `rhel_rhca-node01` [cite: 7] [cite_start]| swap [cite: 9, 60] |
| `/` | [cite_start]37 GiB [cite: 8, 61] | [cite_start]LV en `rhel_rhca-node01` [cite: 7] | [cite_start]XFS [cite: 8] |

---

## ⚙️ Configuración del Sistema

### 1. Selección de Software
[cite_start]Se ha optado por una **"Minimal Install"**[cite: 43]. [cite_start]Esta selección instala únicamente lo estrictamente necesario, optimizando el rendimiento y centrando el aprendizaje en la administración por línea de comandos[cite: 43].

### 2. Registro y Actualización
[cite_start]El sistema debe estar registrado en el portal de Red Hat para acceder a los repositorios oficiales y parches de seguridad[cite: 11, 71].

```bash
# Registro del sistema
sudo subscription-manager register [cite: 11]
sudo subscription-manager attach --auto [cite: 73]

# Actualización completa de paquetes
sudo dnf update -y [cite: 79]
