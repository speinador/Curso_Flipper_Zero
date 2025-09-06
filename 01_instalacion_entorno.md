# ⚙️ Instalación del Entorno

## Inicio
Antes de usar Flipper Zero es necesario configurar el dispositivo y el software base. Primero inserta una tarjeta microSD (recomendado 16–32 GB) en la ranura lateral: en ella se almacenan las claves, tarjetas, controles y datos que leerá Flipper. La tarjeta debe formatearse en FAT32 o exFAT; Flipper la reconocerá automáticamente al encenderlo (tarda más con tarjetas muy grandes)

**Luego actualiza el firmware oficial a la última versión. Existen dos métodos:**

**Aplicación móvil Flipper (iOS/Android):** Activa Bluetooth en el móvil y en Flipper (Menú principal > Ajustes > Bluetooth), empareja y usa la función de actualización integrada. Esto tarda unos minutos y es conveniente para versiones estables.

**Aplicación de escritorio qFlipper:** Descarga e instala qFlipper en tu PC (Windows 10/11, macOS 10.14+ o Linux AppImage). qFlipper instala automáticamente los drivers USB necesarios en Windows. Conecta Flipper por USB-C y desde “Controles avanzados” puedes verificar la versión actual e iniciar la actualización. En Linux recuerda hacer ejecutable el AppImage y configurar las reglas udev.

**En resumen, el laboratorio de instalación incluye:**

- Formatear e insertar microSD.
- Encender Flipper y navegar a Settings para confirmar que reconoce la microSD.
- Instalar qFlipper en el PC (o la app móvil) y actualizar firmware a la versión release.
- Comprobar que Flipper arranca correctamente y muestra fecha/hora (configurable en Settings)


## Introducción a Flipper Zero

Flipper Zero es una herramienta portable tipo “multi-herramienta” para hackers y entusiastas. Integra varias interfaces físicas: radio Sub-GHz, RFID 125 kHz, NFC 13.56 MHz, emisor/receptor infrarrojo, y un puerto USB-C. También dispone de 18 pines GPIO en la parte superior que permiten conectar módulos externos o usarlo como conversor USB-serial/SPI/I²C. Su carcasa sólida y batería recargable lo hacen autónomo; además se puede controlar vía Bluetooth o USB para actualizarlo y transferir datos.

El objetivo de Flipper Zero es aprender y practicar hacking ético en campo de comunicaciones y control de acceso. Por ejemplo, permite escuchar y emular transmisiones Sub-GHz (mando de garaje, sensores, etc.), leer y clonar tarjetas RFID/NFC, controlar dispositivos por IR (TV, aire acondicionado) y actuar como teclado USB HID (Bad USB) para automatizar tareas. Tiene también un simpático “delfín” mascota digital que muestra progreso, animaciones y logros. Su firmware oficial es open source (GPL3), por lo que la comunidad puede ampliar funcionalidades. Sin embargo, es crucial usarlo de forma responsable: el uso sin permiso de sus capacidades (clonación de tarjetas de otros, espionaje, intrusión en sistemas privados) puede ser ilegal.

---
## 🧪 Laboratorio
1. Descarga el software oficial...

---
## 🤔 Reflexión Ética
El uso responsable del dispositivo comienza con...
