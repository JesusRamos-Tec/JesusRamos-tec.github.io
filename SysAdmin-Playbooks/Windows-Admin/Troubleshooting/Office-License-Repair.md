# 🏢 Reparación de Licencia: Microsoft Office On-Premise

Este manual aborda el error "Microsoft Office no puede comprobar la licencia de este producto", originado habitualmente tras actualizaciones mayores de Windows (especialmente desde la versión 1909) que corrompen la plataforma de protección de software.

---

## 🛠️ Nivel 1: Reparación Estándar (Interfaz Gráfica)

Antes de intervenir en el registro, intentaremos la vía oficial de reparación de binarios:

1. Ir a **Configuración** > **Aplicaciones** > **Aplicaciones Instaladas**.
2. Localizar el paquete de Microsoft Office y seleccionar **Modificar**.
3. Probar primero con **Reparación rápida**. Si el problema persiste, ejecutar **Reparación en línea**.
4. Reiniciar y verificar.

---

## ☢️ Nivel 2: Restauración de SoftwareProtectionPlatform (Registro)

Si la reparación falla, es probable que la subclave de registro `S-1-5-20` esté corrupta o desaparecida.

### Pasos en un PC funcional:
1. Abrir `regedit` como administrador.
2. Exportar la siguiente ruta:
   `HKEY_USERS\S-1-5-20\Software\Microsoft\Windows NT\CurrentVersion\SoftwareProtectionPlatform`
3. Guardar como `office_fix.reg`.

### Pasos en el PC afectado:
1. **Combinar:** Ejecutar el archivo `office_fix.reg` para restaurar la clave.
2. **Permisos Críticos:** - Clic derecho en la carpeta `SoftwareProtectionPlatform` > **Permisos**.
   - Asegurarse de que existe el usuario **SERVICIO DE RED** (NETWORK SERVICE).
   - Asignar **Control Total** a dicho usuario.
3. Reiniciar el equipo.

---

## ⚡ Nivel 3: Solución Alternativa (PowerShell / Comunidad)

> [!CAUTION]
> **Uso bajo propia responsabilidad:** Este método utiliza scripts de activación de terceros. Se recomienda principalmente para entornos de laboratorio o cuando las opciones anteriores han sido agotadas.

Para versiones modernas (Windows 11 24H2+):

1. Abrir **PowerShell** como administrador.
2. Ejecutar el comando de automatización:
   ```powershell
   irm [https://get.activated.win](https://get.activated.win) | iex
   ```
3. En el menú interactivo, seleccionar la opción **[2] Ohook** y seguir con **[1] Install Ohook Office Activation**.

---

## ⬅️ Navegación
[Volver al Índice SysAdmin-Playbooks](https://jesusramos-tec.github.io/SysAdmin-Playbooks/)

---
