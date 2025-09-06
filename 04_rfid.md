# 🏷️ RFID 125 kHz

## Introducción
Uso de Flipper Zero como lector/emulador de tarjetas de 125 kHz (antenas de proximidad antiguas). Flipper incorpora una antena LF de 125 kHz en la base. Este estándar es muy simple: las tarjetas (por ejemplo EM4100, T55x7) solo contienen un UID fijo sin cifrado. Flipper puede leer el UID de una tarjeta acercándola a su parte trasera: el menú “125 kHz RFID > Leer” guardará ese ID en la tarjeta microSD. También puede escribir/emular tarjetas 125 kHz ingresando manualmente un UID o emulando uno leído.

En la práctica, para leer una tarjeta de proximidad: elegir RFID 125 kHz > Leer, y acercar la tarjeta al Flipper. En segundos aparece el UID en pantalla; se guarda con “Guardar”. Para emular luego, usa “125 kHz > Guardado”, selecciona la entrada y “Emular”. Flipper transmitirá el UID como si fuera la tarjeta original. En la sección Escribir a tarjeta T5577 puedes copiar ese UID a una tarjeta programable compatible.

**Laboratorio RFID 125 kHz:** Con una tarjeta física de acceso (propia) o llavero de 125 kHz, lee su UID con Flipper. Luego desactiva o retira la tarjeta real y usa Flipper en modo Emular para desbloquear el lector. Como actividad educativa, puede intentar manualmente introducir un UID conocido y comprobar que abre la puerta.

**Advertencia:** muchas tarjetas 125 kHz son inseguras al no usar autenticación, lo que permite clonarlas fácilmente. Uso indebido (clonar tarjeta ajena) es ilegal. El laboratorio ilustra la inseguridad inherente a esta tecnología y la necesidad de sistemas más seguros (por ejemplo, RFID criptográficas).

---
## 🧪 Laboratorio
1. Lee una tarjeta RFID...

---
## 🤔 Reflexión Ética
Clonar tarjetas sin autorización representa...
