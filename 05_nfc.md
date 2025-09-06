# 05_nfc.md

## NFC (13.56 MHz)

Flipper Zero incluye un módulo NFC de alta frecuencia (13.56 MHz) basado en el chip ST25R3916 con antena HF compartida junto a la antena LF:contentReference[oaicite:46]{index=46}:contentReference[oaicite:47]{index=47}. Este módulo permite **leer, guardar, emular y escribir tarjetas NFC** (por ejemplo MIFARE Classic, NTAG, tarjetas de transporte, pases de acceso) y tags NFC. A diferencia del RFID 125 kHz, las tarjetas NFC usan protocolos más complejos con cifrado y autenticación bidireccional:contentReference[oaicite:48]{index=48}. Flipper puede leer datos básicos de la tarjeta (UID, SAK, ATQA, contenido almacenado) y realizar operaciones avanzadas como *recuperar llaves MIFARE Classic* mediante la emulación de tarjetas para extraer nonces criptográficos:contentReference[oaicite:49]{index=49}.

En el menú **NFC**, elija *Leer*. Acerque la tarjeta NFC a la parte trasera del Flipper; este mostrará UID, ATQA, SAK y cualquier dato legible en la pantalla. Para guardar, seleccione *Guardar* y asigne un nombre. El Flipper puede emular tarjetas NFC guardadas mediante la opción *Guardadas* → *Emular*. Además, dispone de opciones extra para ataques a MIFARE Classic: al activar *Recuperar llaves MIFARE*, Flipper emula una tarjeta para obtener nonces usados por el lector y luego calcula las llaves secretas (este proceso puede tomar tiempo). 

## Laboratorio práctico

1. Coloque una tarjeta NFC compatible (p.ej., MIFARE Classic de 1K) cerca de la parte trasera del Flipper. En el menú **NFC**, seleccione *Leer*.  
2. Observe que Flipper muestra la información básica de la tarjeta (UID, SAK, ATQA, etc.). Pulse *Guardar* para almacenar estos datos (por ejemplo, “Tarjeta Test”).  
3. Pruebe la emulación: en el menú NFC seleccione *Guardadas*, elija “Tarjeta Test” y pulse *Emular*. Acérquese al lector original de la tarjeta (por ejemplo, un controlador de puerta). Flipper intentará actuar como si fuera esa tarjeta. Verifique si el sistema acepta la emulación.  
4. (Opcional, bajo autorización) Intente la función *Recuperar llaves MIFARE*: diríjase a *Más → Recuperar MIFARE Classic*. Siga las instrucciones para capturar datos criptográficos. Este paso ilustra cómo se pueden auditar las seguridades de tarjetas MIFARE Classic.

## Reflexión ética

Las tarjetas NFC suelen contener información personal sensible (por ejemplo, datos de transporte público o llaves de edificio). Usar el Flipper Zero para **clonar o analizar tarjetas NFC de terceros sin permiso** vulnera la privacidad y la seguridad, constituyendo una práctica ilegal:contentReference[oaicite:50]{index=50}. Siempre utilice NFC en tarjetas que le pertenezcan o en entornos de prueba controlados. No intente interferir con sistemas de pago o datos confidenciales. Si practica la recuperación de claves MIFARE, hágalo únicamente con tarjetas de prueba propias y procurando no afectar a usuarios legítimos. En resumen, respete la ley y los derechos de terceros al manipular tarjetas NFC con el Flipper Zero.
