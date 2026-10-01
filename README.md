# 🧩 AlphaNet v0.4 - WAN Tools Suite (Corte 2)

**Autor:** [Kevin Camilo Ramos Villamil]  
**Institución:** [U Compensar]  
**Asignatura:** [Interconexion de redes Wan]  
**Docente:** [John Harold Pérez Calderón]  
**Fecha:** 2026  
**Repositorio:** https://github.com/[tu-usuario]/wan-tools-alphanet

---

## 📋 Descripción

**AlphaNet v0.4** es una herramienta web de diseño y gestión de redes WAN que integra 7 módulos funcionales para administrar infraestructura de red multi-vendor. Desarrollada como parte del **Corte 2**, cumple con los 4 requisitos solicitados:

1. ✅ **Subnetting IPv4 + VLSM** — Calculadora y planificación de direccionamiento
2. ✅ **Carga de Topología WAN** — Gestión de dispositivos multi-vendor
3. ✅ **Generación de Configuraciones** — Cisco, Huawei, Fortinet y MikroTik
4. ✅ **Ciberdefensa contra IA** — Análisis de amenazas y contramedidas

---

## 🎯 Características

### 🖥️ Módulo 1: Dashboard
- Tarjetas KPI (dispositivos, fabricantes, protocolos, ancho de banda)
- Panel de latencia con gráficos en tiempo real
- Tabla de dispositivos con estados y acciones
- Terminal de logs interactiva

### ⚙️ Módulo 2: Configuración de Equipos
- Soporte multi-vendor: **Cisco, Huawei, TP-Link, Fortinet, MikroTik**
- Selección por tipo: Router, Switch L2, Switch L3, Firewall, AP
- Configuración de VLANs, interfaces, routing y seguridad
- Vista previa de sintaxis específica por fabricante

### 📋 Módulo 3: Plantillas
- 8 plantillas prediseñadas listas para usar
- Carga con un clic en el editor de configuración

### 🚀 Módulo 4: Despliegue
- Despliegue a 1 dispositivo, grupo, masivo o programado
- Backup automático antes de aplicar cambios

### 📐 Módulo 5: Subnetting
- Cálculo completo de subredes IPv4 (CIDR)
- Máscara, red, broadcast, rango de hosts
- Plan VLSM automático según requerimientos

### 🗺️ Módulo 6: Topología WAN
- Carga manual o demo de dispositivos
- Gestión de IPs de gestión, WAN y LAN
- Generación de configuración desde la topología

### 🛡️ Módulo 7: Ciberdefensa contra IA
- Análisis de 4 tipos de amenazas con IA:
  - Reconocimiento con IA
  - DDoS adaptativo
  - Phishing generativo
  - Malware polimórfico
- Contramedidas recomendadas
- Checklist de seguridad

---

## 🚀 Uso

1. Abre `index.html` en Chrome (o cualquier navegador moderno)
2. No requiere instalación ni dependencias
3. Navega por las 7 pestañas del menú superior

---

## 📸 Tabla de Evidencias

| # | Evidencia | Archivo | Estado |
|---|-----------|---------|--------|
| 1 | Subnetting IPv4 + VLSM funcional | `docs/capturas/01-subnetting.png` | ✅ |
| 2 | Carga de topología WAN (6 dispositivos) | `docs/capturas/02-topologia.png` | ✅ |
| 3 | Configuración Cisco generada | `docs/capturas/03-config-cisco.png` | ✅ |
| 4 | Configuración Huawei generada | `docs/capturas/04-config-huawei.png` | ✅ |
| 5 | Historial de commits en GitHub | `docs/capturas/05-github-commits.png` | ✅ |

---

## 📁 Estructura del Repositorio
wan-tools-alphanet/
├── README.md
├── .gitignore
├── index.html
└── docs/
├── informe-corte2.pdf
└── capturas/
├── 01-subnetting.png
├── 02-topologia.png
├── 03-config-cisco.png
├── 04-config-huawei.png
└── 05-github-commits.png

---

## 🔒 Política de Seguridad

- ❌ **Nunca** subir contraseñas, tokens o API keys al repositorio
- ✅ Usar `.gitignore` para excluir archivos `.env`
- ✅ Toda la actividad se realiza sobre infraestructura autorizada del laboratorio

---

## 🛠️ Tecnologías Utilizadas

- **HTML5** — Estructura
- **CSS3** — Estilos y responsive design
- **JavaScript (ES6)** — Lógica de negocio
- **Git** — Control de versiones

---

## 📚 Bibliografía

- Cisco Systems. (2024). *Cisco IOS Configuration Fundamentals*.
- Huawei Technologies. (2024). *VRP Configuration Guide*.
- Fortinet. (2024). *FortiOS Administration Guide*.
- MikroTik. (2024). *RouterOS Manual*.
- Odom, W. (2020). *Cisco CCNA 200-301 Official Cert Guide*. Cisco Press.
- Tanenbaum, A. S. (2021). *Computer Networks* (6th ed.). Pearson.

---

## 📄 Licencia

Proyecto académico — Corte 2 — 2026
