# Pruebas de la Aplicación - AlphaNet v1.6

**Entorno:** Google Chrome (Windows)  
**Resultado:** 11/11 pruebas exitosas (100% de confianza)

| # | Módulo | Descripción | Resultado |
|---|--------|-------------|-----------|
| P1 | Dashboard | Muestra "No hay dispositivos" al inicio. | ✅ |
| P2 | Topología | Agregar Router Cisco aparece en Tabla y Dashboard. | ✅ |
| P3 | Persistencia | Recargar la página mantiene el equipo. | ✅ |
| P4 | Persistencia | Eliminar equipo y recargar lo borra definitivamente. | ✅ |
| P5 | Configuración | Cisco Switch L2 usa `Fa0/1` y respeta campos DNS vacíos. | ✅ |
| P6 | Configuración | Fortinet incluye NTP, Password Policy y SSH v2. | ✅ |
| P7 | Configuración | MikroTik (Switch) incluye `bridge` y `vlan-filtering=yes`. | ✅ |
| P8 | Configuración | Botón de exportación descarga el archivo `.txt`. | ✅ |
| P9 | Subnetting | Calcula red y broadcast correctamente (`192.168.1.10/24`). | ✅ |
| P10| Ciberdefensa | Analiza amenazas y sugiere contramedidas. | ✅ |
| P11| Ciberdefensa | Valida nombre de equipo y alerta sobre Telnet. | ✅ |