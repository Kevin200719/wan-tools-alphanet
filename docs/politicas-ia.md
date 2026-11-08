# Políticas de Ciberseguridad y Uso de IA - AlphaNet v1.6

La herramienta AlphaNet ha sido diseñada bajo los principios de **Zero Trust** y **Ciberseguridad Activa**.

## 1. Políticas de Configuración Segura
- **SSH v2 Obligatorio:** Se fuerza el uso de SSH versión 2. El protocolo Telnet está deshabilitado por defecto.
- **Complejidad de Contraseñas:** Los generadores incluyen políticas de contraseñas de al menos 12 caracteres.
- **Protección de Capa 2:** En switches Cisco, se habilita `bpduguard` y `portfast` para evitar bucles.

## 2. Políticas de Ciberdefensa contra IA
- **Validación de Entradas:** Se bloquean nombres de equipos con caracteres maliciosos o espacios.
- **Advertencia de Configuraciones Inseguras:** Si el usuario intenta habilitar Telnet, la aplicación lanza una alerta de seguridad.
- **Cero Persistencia de Secretos:** AlphaNet no guarda contraseñas ni claves en localStorage.
- **Análisis de Amenazas:** Simula ataques (DDoS, Phishing, Malware) y entrega contramedidas (BGP Flowspec, uRPF, QoS).