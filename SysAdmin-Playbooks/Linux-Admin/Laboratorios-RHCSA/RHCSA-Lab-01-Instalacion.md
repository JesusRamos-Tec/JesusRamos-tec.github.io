# 🐧 Lab 01: Instalación y Configuración Base de RHEL 9.7

Este manual documenta el proceso detallado de instalación, configuración inicial y preparación del entorno de laboratorio para la certificación **RHCSA**[cite: 1, 38].

## 🏗️ Entorno del Laboratorio
El despliegue se realiza sobre un nodo de virtualización **Proxmox VE 9.0.3** ejecutándose en un hardware **BMAX Pro** con 32GB de RAM y 1TB de disco duro[cite: 3].

### Especificaciones de la VM (rhca-labs)
* **CPU**: 1 Socket / 2 Cores (Tipo: Host para acceso real al microprocesador)[cite: 4, 30].
* **RAM**: 4GB (4096MB)[cite: 4, 31].
* **Disco**: 40GB (VirtIO)[cite: 4, 28].
* **Sistema**: Qemu Agent habilitado para gestión desde el hipervisor[cite: 27].

---

## 💾 Gestión de Almacenamiento (LVM)
Se aplica un particionado manual basado en **Logical Volume Management (LVM)** para garantizar flexibilidad en la gestión de volúmenes[cite: 5, 56, 57].

| Punto de Montaje | Tamaño | Tipo / Volume Group | Sistema de Archivos |
| :--- | :--- | :--- | :--- |
| `/boot` | 1024 MiB | Partición Estándar | XFS |
| `swap` | 2 GiB | LV en `rhel_rhca-node01` | swap |
| `/` | 37 GiB | LV en `rhel_rhca-node01` | XFS |

---

## ⚙️ Configuración del Sistema

### 1. Selección de Software
Se ha optado por una **"Minimal Install"**. Esta selección instala únicamente lo estrictamente necesario, optimizando el rendimiento y centrando el aprendizaje en la administración por línea de comandos.

### 2. Registro y Actualización
El sistema debe estar registrado en el portal de Red Hat para acceder a los repositorios oficiales y parches de seguridad.

```bash
# Registro del sistema
sudo subscription-manager register [cite: 11]
sudo subscription-manager attach --auto [cite: 73]

# Actualización completa de paquetes
sudo dnf update -y [cite: 79]
```

### 3. Herramientas de Administración
[cite_start]Instalación del kit básico de supervivencia para el administrador[cite: 80]:

* [cite_start]**`vim`**: Editor de archivos de configuración (equivalente a nano)[cite: 83].
* [cite_start]**`bash-completion`**: Permite completar comandos automáticamente pulsando la tecla **Tab**[cite: 84].
* [cite_start]**`net-tools`**: Incluye utilidades clásicas de red como `ifconfig` o `netstat`[cite: 85].
* [cite_start]**`wget` / `curl`**: Herramientas imprescindibles para la descarga de recursos y archivos directamente desde la web al servidor[cite: 86].
