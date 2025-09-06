# 📡 Sub-GHz

## Introducción
Flipper leyendo una señal Sub-GHz (por ejemplo, de una barrera de garaje). Su módulo de radio CC1101 integrado cubre 300–928 MHz con antena multi-banda, alcanzando unos 50 m de rango en campo abierto. Por defecto puede capturar y decodificar controles remotos comunes de 315/433/868 MHz (cuando son protocolos conocidos), o guardar la señal en formato RAW para intentar reproducirla luego.

mm

Al elegir Sub-GHz > Leer en Flipper, presiona el botón del control remoto a pocos centímetros: Flipper detectará la frecuencia (~433.92 MHz, por ejemplo) y mostrará en pantalla la señal capturada. Si no la decodifica automáticamente, se graba como RAW. Puedes luego enviar esa señal guardada con Enviar. En la configuración de Sub-GHz puedes ajustar manualmente la frecuencia (usar el analizador de frecuencias para encontrar la más alta) y la modulación (AM/FM/OOK/ASK, etc.). Existe un modo analizador donde Flipper barre varias frecuencias y te muestra la más fuerte, o un modo hopping que explora rangos automáticamente.

Laboratorio Sub-GHz: El alumno puede practicar capturando el código de un control remoto (ej. puerta de garaje o luz remota de jardín). Pasos:

1. Seleccionar Sub-GHz > Leer, presionar el botón del control remoto cerca de Flipper.
2. Guardar la señal grabada con un nombre significativo.
3. Ir a Sub-GHz > Guardadas, seleccionar la señal y “Enviar” para reproducirla.
4. Observar que el dispositivo responde igual que con el control original.
5. Probar cambiar manualmente la frecuencia o modulación si hay problemas.

**Posibles usos ilegítimos:** clonar controles de acceso sin autorización para abrir puertas o coches. ¡Precaución! Esto puede constituir delito. El objetivo del laboratorio es entender el mecanismo, no eludir permisos.

---

## 🧪 Laboratorio
1. Captura una señal de control remoto...

---
## 🤔 Reflexión Ética
Transmitir señales ajenas sin permiso puede...
