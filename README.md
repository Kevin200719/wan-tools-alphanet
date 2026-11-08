# 🧩 AlphaNet v1.6 - WAN Tools Suite (Corte 3)

**Autor:** [Tu Nombre Completo]  
**Institución:** [Nombre de tu Universidad]  
**Asignatura:** [Nombre de la materia]  
**Docente:** [Nombre del profesor]  
**Fecha:** Noviembre 2026  
**Repositorio:** https://github.com/Kevin200719/wan-tools-alphanet

---

## 📋 Descripción

**AlphaNet v1.6** es una herramienta web de diseño y gestión de redes WAN que integra múltiples módulos funcionales para administrar infraestructura de red multi-vendor. Esta versión (Corte 3) incorpora mejoras críticas de persistencia, ciberseguridad y usabilidad.

### 🚀 Novedades del Corte 3 (v1.6)
1. **Persistencia de Datos:** La topología se guarda automáticamente en el navegador (`localStorage`), evitando perder el progreso al recargar.
2. **Dashboard Dinámico:** Muestra únicamente los equipos reales de la topología, eliminando latencias simuladas.
3. **Validaciones de Ciberdefensa:** Bloquea nombres de equipos inválidos y alerta sobre el uso de protocolos inseguros como Telnet.
4. **Exportación de Configuraciones:** Genera un archivo descargable (`.txt`) con la configuración lista para aplicar en el equipo físico o simulado.
5. **Documentación Completa:** Manual de usuario, políticas de IA y registro de pruebas incluidos en la carpeta `docs/`.

---

## 🎯 Características Principales

- **Multi-Vendor:** Soporte para Cisco, Huawei, TP-Link, Fortinet y MikroTik.
- **Generación por Rol:** Configuraciones específicas para Router, Switch L2, Switch L3, Firewall y AP.
- **Ciberdefensa:** Análisis de amenazas potenciadas por IA y contramedidas.
- **Subnetting y VLSM:** Calculadora de redes IPv4 y planificación de direccionamiento.
- **Visualización:** Diagrama SVG de la topología de red.

---

## 📸 Tabla de Evidencias (Corte 3)

| # | Evidencia | Archivo | Estado |
|---|-----------|---------|--------|
| 1 | Subnetting IPv4 + VLSM | `docs/capturas/01-subnetting.png` | ✅ |
| 2 | Carga de topología WAN | `docs/capturas/02-topologia.png` | ✅ |
| 3 | Configuración Cisco | `docs/capturas/03-config-cisco.png` | ✅ |
| 4 | Configuración Huawei | `docs/capturas/04-config-huawei.png` | ✅ |
| 5 | Historial de commits (Corte 2) | `docs/capturas/05-github-commits.png` | ✅ |
| 6 | Configuración Fortinet | `docs/capturas/06-config-fortinet.png` | ✅ |
| 7 | Configuración MikroTik | `docs/capturas/07-config-mikrotik.png` | ✅ |
| 8 | Módulo de Ciberdefensa | `docs/capturas/08-ciberdefensa.png` | ✅ |
| 9 | Pruebas al 100% de éxito | `docs/capturas/09-pruebas.png` | ✅ |
| 10 | Historial de commits (Corte 3) | `docs/capturas/10-commits-corte3.png` | ✅ |

---

## 📁 Estructura del Repositorio

```text
wan-tools-alphanet/
├── README.md
├── index.html                      (Aplicación AlphaNet v1.6)
└── docs/
    ├── informe-corte3.pdf          (Informe final actualizado)
    ├── manual-usuario.md           (Manual corporativo)
    ├── politicas-ia.md             (Políticas de ciberseguridad)
    ├── pruebas.md                  (Registro de las 11 pruebas)
    └── capturas/                   (Evidencias 01 a 10)
  
🚀 Uso
Abre index.html en Chrome (no requiere instalación).

Navega por las pestañas para configurar tu red.

Genera y descarga las configuraciones en formato .txt.

🔒 Política de Seguridad
❌ Nunca se suben contraseñas ni tokens reales al repositorio.

✅ Uso de .gitignore para excluir archivos .env.

✅ Políticas de Zero Trust aplicadas en la generación de configuraciones.

📚 Bibliografía
Cisco Systems. (2024). Cisco IOS Configuration Fundamentals.

Huawei Technologies. (2024). VRP Configuration Guide.

Fortinet. (2024). FortiOS Administration Guide.

MikroTik. (2024). RouterOS Manual.

NIST. (2024). Zero Trust Architecture (SP 800-207).

