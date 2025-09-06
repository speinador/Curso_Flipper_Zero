# 03_subghz.md

## Sub-GHz (Radiofrecuencia)

El Flipper Zero cuenta con un módulo de radiofrecuencia integrado (basado en el chip CC1101) que opera en el rango de **300–928 MHz**. Esto le permite **leer, guardar y emular controles remotos** de muchos dispositivos inalámbricos comunes:contentReference[oaicite:37]{index=37}:contentReference[oaicite:38]{index=38}. Estos controles incluyen mandos de **puertas de garaje, portones, barreras, interruptores remotos, timbres inalámbricos, luces inteligentes**, entre otros. Gracias a este módulo Sub-GHz, Flipper puede “aprender” la señal de estos dispositivos y reproducirla, lo que sirve para verificar la seguridad de sistemas que usan RF.

![plot](https://github.com/speinador/Curso_Flipper_Zero/blob/main/img/Sub-GHz.png)

En la aplicación Sub-GHz del Flipper puede seleccionar **Leer** para capturar el código de un control remoto conocido (si el protocolo es compatible, guarda inmediatamente el ID; si no, lo guarda en formato RAW). También hay modos como **Analizador de frecuencias** para determinar la frecuencia exacta de la señal capturada. Flipper Zero soporta frecuencias en bandas comunes: 300-348 MHz, 387-464 MHz y 779-928 MHz:contentReference[oaicite:39]{index=39}. El dispositivo incluye antena interna (alcance ~50 metros) y permite conectar antenas externas para mayor alcance:contentReference[oaicite:40]{index=40}. Además, puede crear controles virtuales manualmente o ajustar la codificación (ASK/FSK) en caso de que la lectura falle.

## Laboratorio práctico

1. Encienda el Flipper y vaya al menú **Sub-GHz**. Elija *Leer* y, cuando le pida, presione un botón de un mando remoto (p.ej., control de garaje) cercano al Flipper. Espere hasta que aparezca “Capture OK” (o similar) en la pantalla.  
2. Seleccione *Guardar* (More → Save) para almacenar la señal con un nombre reconocible.  
3. Vuelva al menú Sub-GHz, entre en *Emulados* (Saved) y seleccione el control recién grabado. Pulse *Emular* y acerque el Flipper al lector (puerta o dispositivo). El Flipper enviará la señal guardada; verifique que el dispositivo responde (p. ej., la puerta abre).  
4. Pruebe el **Analizador de frecuencias**: mantenga pulsado el mando remoto a varios metros del Flipper, y en Sub-GHz seleccione *Analizador* para que muestre la frecuencia con mayor RSSI. Observe cómo cambia la lectura según la distancia.  
5. Experimente agregando manualmente un control (Add Manually): especifique un valor de frecuencia y pulse *FREQ Analyzer* para calibrar si conoce el protocolo.

## Reflexión ética

El uso del radio Sub-GHz puede vulnerar sistemas de seguridad si se hace sin permiso. Según INCIBE, un riesgo grave es el «acceso no autorizado» a sistemas:contentReference[oaicite:41]{index=41}. Por ello, **solo grabe y emule controles que sean de su propiedad o para los que tenga autorización**. Por ejemplo, emular su propio mando de garaje para pruebas de seguridad está permitido, pero emular el de un vecino o un edificio ajeno sería ilegal. Evite interferir con transmisiones de emergencia o canales restringidos. En resumen, respete siempre la legislación de radiofrecuencia local y solo use Flipper Sub-GHz con fines educativos o de auditoría autorizada.
