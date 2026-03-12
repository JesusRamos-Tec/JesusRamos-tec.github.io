# Anexo 24: Gestión de Logs y Monitorización

## 🎯 Objetivo
Determinar los eventos significativos dentro de los sistemas de información que deben ser registrados y establecer mecanismos de monitorización que permitan la detección temprana de intrusiones, errores o comportamientos anómalos.

---

## 🔍 Definición de la Actividad Registrada

Para garantizar la trazabilidad y la seguridad, se auditan de forma obligatoria los siguientes eventos:

### 1. Eventos de Acceso y Gestión de Información
* **Acceso a datos:** Creación, borrado y actualización de información clasificada como confidencial.
* **Sesiones de usuario:** Inicio y fin de conexión en la red corporativa, así como intentos de inicio de sesión fallidos.
* **Privilegios:** Modificaciones en los permisos de acceso y cambios en configuraciones críticas de sistemas.

### 2. Salud del Sistema y Aplicativos
* **Rendimiento:** Uso de CPU, memoria, capacidad de disco y ancho de banda.
* **Errores:** Ejecución o finalización anómala de aplicaciones y servicios.
* **Seguridad activa:** Indicios de actividad sospechosa detectada por Antivirus o Sistemas de Detección de Intrusos (IDS).

---

## 📋 Estructura y Protección del Log

Cada registro generado debe incluir, como mínimo, la siguiente información para facilitar su análisis:
* **Identificación:** ID del usuario, dirección IP/MAC del dispositivo y protocolos utilizados.
* **Temporalidad:** Fecha y hora exacta del evento (requiere **Sincronización de Reloj** mediante NTP).
* **Contexto:** Tipología del evento y elemento afectado (ficheros, bases de datos, equipos).

> [!IMPORTANT]
> **Protección y Almacenamiento:** Los logs deben protegerse contra modificaciones no autorizadas y almacenarse durante el periodo legal establecido para garantizar su validez en procesos de forense digital.

---

## 📊 Matriz de Control de Gestión de Logs

| NIVEL | ALCANCE | CONTROL DE SEGURIDAD | ESTADO |
| :---: | :---: | :--- | :---: |
| **B** | **PRO** | Definición de actividades críticas sujetas a registro. | ☐ |
| **B** | **PRO** | Determinación de la información relevante a incluir en cada log. | ☐ |
| **B** | **PRO** | Estandarización del formato de logs para análisis posterior. | ☐ |
| **A** | **TEC** | Selección e implementación del mecanismo de registro centralizado. | ☐ |
| **B** | **TEC** | Medidas de protección y cifrado del almacenamiento de logs. | ☐ |
| **B** | **TEC** | Sincronización horaria (NTP) en todos los nodos de la red. | ☐ |
| **B** | **TEC** | Configuración de alertas en tiempo real ante comportamientos anómalos. | ☐ |

**Revisado por:** ___________________________  
**Fecha:** __________

---

## ⬅️ Navegación
[Volver al Índice ISO27001](https://jesusramos-tec.github.io/ISO27001-Framework/)

---


## 🚀 Implementación Técnica Recomendada
Para dar cumplimiento a este anexo, se recomienda el despliegue de una solución de tipo **SIEM (Wazuh)** que permita centralizar estos registros, correlacionar eventos de seguridad y generar alertas automáticas ante picos de rendimiento o cambios en configuraciones críticas.
