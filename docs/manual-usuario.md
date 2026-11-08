# MANUAL DE USUARIO
## AlphaNet v1.6 - Network Command Center

**Versión del documento:** 1.0  
**Fecha de emisión:** Noviembre 2026  
**Clasificación:** Uso interno / Documentación técnica  
**Desarrollador:** Kevin [Tu Apellido]  

---

## 1. Introducción

Bienvenido a **AlphaNet**, la herramienta de orquestación y diseño de redes WAN multi-vendor. Este manual está diseñado para guiar a los ingenieros de red y administradores de sistemas en el uso correcto de la plataforma para automatizar la generación de configuraciones, calcular subredes y aplicar políticas de ciberdefensa.

AlphaNet no requiere instalación de software adicional; funciona directamente en el navegador web.

---

## 2. Requisitos del Sistema

- **Navegador Web:** Google Chrome (versión 90+), Microsoft Edge o Firefox.
- **Sistema Operativo:** Windows, macOS o Linux.
- **Resolución mínima:** 1366 x 768 px.
- **Conectividad:** No requiere internet para funcionar (excepto para los enlaces externos a documentación oficial).

---

## 3. Acceso a la Herramienta

1. Ubique el archivo `index.html` en el directorio del proyecto.
2. Haga doble clic sobre el archivo o ábralo arrastrándolo hacia su navegador web.
3. La interfaz principal (Dashboard) se cargará automáticamente.

---

## 4. Interfaz Principal (Dashboard)

El Dashboard es el centro de control. Muestra un resumen en tiempo real de los equipos cargados en la topología.

- **Tarjeta de Dispositivos:** Indica el total de equipos en la topología activa.
- **Tarjeta de Fabricantes:** Muestra cuántas marcas distintas (Cisco, Huawei, etc.) están en uso.
- **Tabla de Equipos:** Lista los equipos agregados con su nombre, IP y fabricante.
- **Persistencia:** La herramienta guarda automáticamente la topología en la memoria del navegador. Si cierra la pestaña y la vuelve a abrir, sus equipos seguirán ahí.

---

## 5. Módulos de Trabajo

### 5.1. Topología WAN
Antes de generar configuraciones, debe definir su red.
1. Vaya a la pestaña **"🗺️ Topología WAN"**.
2. Rellene los campos: Nombre del equipo, Fabricante, Tipo (Router, Switch, Firewall), IP de Gestión, IP WAN y IP LAN.
3. Haga clic en **"➕ Agregar"**. El equipo aparecerá en el diagrama y en el Dashboard.
4. Para pruebas rápidas, puede hacer clic en **"📋 Cargar Demo"** para cargar una red de ejemplo.

### 5.2. Generación de Configuraciones
1. Vaya a la pestaña **"⚙️ Configuración"**.
2. Seleccione el **Fabricante** (Cisco, Huawei, TP-Link, Fortinet o MikroTik).
3. Seleccione el **Tipo de Dispositivo** (Router, Switch L2, Switch L3, Firewall, AP).
4. Seleccione el **Modelo Específico** (Esto adapta la sintaxis de las interfaces, por ejemplo `Fa0/1` en un 2960).
5. Complete los parámetros generales (DNS, NTP, Dominio, etc.).
6. En la pestaña **VLANs** e **Interfaces**, defina la segmentación de su red.
7. Haga clic en el botón **"⚡ Generar"**.
8. En la pestaña **"👁️ Vista Previa"**, verá el código generado. Puede usar el botón **"💾 Descargar"** para obtener el archivo `.txt` y aplicarlo en su equipo.

### 5.3. Calculadora de Subnetting y VLSM
1. Vaya a la pestaña **"📐 Subnetting"**.
2. Para calcular una subred, ingrese la IP con su prefijo (ej: `192.168.1.10/24`) y haga clic en **"Calcular"**.
3. Para generar un plan VLSM, ingrese la red base y los hosts requeridos separados por coma (ej: `50, 25, 10`). Haga clic en **"Generar VLSM"**.
4. Puede descargar el plan de direccionamiento en un archivo `.txt`.

### 5.4. Ciberdefensa IA
1. Vaya a la pestaña **"🛡️ Ciberdefensa IA"**.
2. Seleccione el tipo de amenaza (Reconocimiento, DDoS, Phishing, Malware).
3. Seleccione el nivel de riesgo.
4. Haga clic en **"Analizar"** para ver el impacto en su red.
5. Haga clic en **"Aplicar Contramedidas"** para recibir las recomendaciones de seguridad.

---

## 6. Políticas de Seguridad Integradas (Ciberdefensa)

AlphaNet aplica controles de seguridad de forma automática:
- **Validación de Entradas:** Si intenta poner un nombre de equipo con espacios (ej: `SW CORE`), la app lo bloqueará y le pedirá usar guiones (`SW-CORE`).
- **Alerta de Telnet:** Si intenta generar una configuración con Telnet habilitado, la app lanzará una alerta roja advirtiendo que es un protocolo inseguro.
- **Sin Guardado de Secretos:** La herramienta no guarda contraseñas ni tokens en el navegador; todo se genera en memoria.

---

## 7. Preguntas Frecuentes (FAQ)

**¿La herramienta se conecta directamente a mis equipos?**
No. AlphaNet genera el código de configuración. Usted debe copiarlo (o descargarlo) y aplicarlo manualmente en el equipo vía consola o SSH.

**¿Por qué la configuración de Cisco usa `Fa0/1` y no `Gi1/0/1`?**
Depende del modelo. Si selecciona un *Catalyst 2960*, usará `Fa0/1`. Si selecciona un *3560*, usará `Gi1/0/1`. La app adapta la sintaxis automáticamente.

**¿Qué pasa si cierro el navegador?**
La topología se guarda en la memoria local (localStorage). Al abrir de nuevo la app, sus equipos seguirán ahí.

---
*Fin del manual. Para soporte técnico, contacte al administrador del sistema.*