# 📡 Infrarrojos

## Introducción
Flipper Zero puede capturar y emitir señales infrarrojas de controles remotos. Tiene integrados IR LEDs de emisión y receptor tras la carcasa. En el menú Infrarrojos > Aprender apuntas tu control remoto normal al Flipper y presionas un botón: Flipper guardará la señal codificada (por ejemplo, código NEC, RC5, etc.) asociada a ese botón. En Ir Aplicaciones > Control universales Flipper puede también enviar códigos precargados de su base de datos interna para muchos aparatos comunes (TV, aire acondicionado, estéreo). Este modo recorre automáticamente todos los protocolos conocidos (“ataque por diccionario”).

![plot](https://github.com/speinador/Curso_Flipper_Zero/blob/main/img/Infrarrojos.png)

Para enviar una señal aprendida, ve a Infrarrojos > Guardados, selecciona el dispositivo y botón deseado, y usa “Enviar”. Flipper transmitirá la secuencia infrarroja exactamente como el control original. La interfaz permite administrar colecciones de mandos: por marca/dispositivo. Gracias a la comunidad, su base de datos de códigos IR está en constante expansión.

**Laboratorio IR:** Con un control remoto de TV o aire acondicionado, practica “Aprender” cada botón con Flipper. Luego apaga el dispositivo original y usa Flipper en Universal Remote o enviando los comandos guardados para controlar el equipo. Además, explora el modo “Universal”: selecciona un dispositivo (p.ej. Samsung TV) y prueba cambiar volumen o canales. Uso indebido: controlar dispositivos de terceros sin permiso (por ejemplo apagar TVs de desconocidos) es inmoral e intrusivo. El fin es entender la tecnología IR y aprender que muchos controles pueden ser clonados con facilidad.

---
## 🧪 Laboratorio
1. Captura un comando de un control remoto IR...

---
## 🤔 Reflexión Ética
Usar controles IR ajenos sin autorización...
