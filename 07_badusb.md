# ⌨️ Bad USB

## Introducción
Flipper Zero puede actuar como dispositivo BadUSB, es decir simular un teclado o ratón USB para inyectar comandos en un ordenador anfitrión. Utiliza el lenguaje de scripting tipo Rubber Ducky (Duckyscript) para escribir payloads: secuencias de teclas automáticas. Por ejemplo, un payload típico puede abrir una terminal, ejecutar comandos o descargar archivos sin intervención del usuario. Flipper reconoce una carpeta especial en la microSD (/badusb/) donde colocas archivos .txt con tu script. Luego, en Bad USB, seleccionas el script y conectas Flipper por USB (cable-C) en modo HID. Al presionar “Run”, Flipper envía las pulsaciones según el guión.

Por ejemplo, un payload sencillo puede hacer que Flipper abra el Bloc de notas y escriba “¡Hola mundo!” o que ejecute instrucciones de PowerShell. Flipper soporta atajos avanzados (Alt+numpad, combinaciones rápidas, etc.). También es posible conectar vía Bluetooth (BLE) como un teclado inalámbrico para ejecutar scripts si el PC lo permite. Es fundamental entender que BadUSB es poderoso: puede crear puertas traseras, robar contraseñas o instalar malware si se abusa. Su uso debe limitarse a entornos de prueba bajo consentimiento.

**Laboratorio BadUSB:** Crea un script básico (por ejemplo, abre calculadora o escribe texto) usando Duckyscript y guárdalo en un archivo .txt. Carga el archivo en la tarjeta SD bajo /badusb/. En Flipper, ve a Bad USB, selecciona el modo USB o BLE, ajusta el layout de teclado si es necesario, y ejecuta el payload conectado a un PC de pruebas. Verifica que Flipper logra automatizar las teclas esperadas. Discute los peligros: este método es análogo a un USB Rubber Ducky.

---
## 🧪 Laboratorio
1. Configura un payload Rubber Ducky básico...

---
## 🤔 Reflexión Ética
Los ataques con BadUSB son peligrosos...
