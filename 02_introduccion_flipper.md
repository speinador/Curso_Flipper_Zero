# 02_introduccion_flipper.md

## ¿Qué es Flipper Zero?

Flipper Zero es un dispositivo multifuncional diseñado para entusiastas de la seguridad y la electrónica. Se presenta en forma de llavero con pantalla táctil, botones y una serie de sensores integrados, pensado «para explorar, aprender y experimentar con tecnologías de comunicación inalámbrica, sistemas de seguridad y dispositivos electrónicos»:contentReference[oaicite:32]{index=32}. Gracias a su hardware abierto y firmware personalizable, Flipper Zero permite realizar tareas como lectura/emulación de tecnologías RFID, NFC, Bluetooth, Infrarrojos y radiofrecuencia.

La versatilidad del Flipper Zero es amplia: **pruebas de penetración en sistemas de seguridad**, clonación de tarjetas de acceso, control de dispositivos IR (televisores, aires acondicionados, etc.), análisis de señales de radio y otras actividades relacionadas con ciberseguridad:contentReference[oaicite:33]{index=33}. Aunque su objetivo declarado es educativo (mejorar habilidades de hacking y ciberseguridad), es preciso usarlo de manera **legal y ética**. No está destinado a actividades maliciosas, pero un uso indebido puede conllevar riesgos como el acceso no autorizado a sistemas o daño a dispositivos ajenos:contentReference[oaicite:34]{index=34}:contentReference[oaicite:35]{index=35}.

## Laboratorio práctico

1. **Actualice el firmware:** Conecte y empareje el Flipper con la app móvil o qFlipper como en el módulo anterior. Asegúrese de instalar la última versión oficial (esto habilita nuevas funciones y parches de seguridad).  
2. **Conozca el menú principal:** Navegue por el Menú Principal del Flipper Zero para familiarizarse con las secciones básicas: Sub-GHz, 125 kHz RFID, NFC, Infrarrojos, GPIO, Bad USB, etc.  
3. **Experimente con demos básicas:** En la sección **Sub-GHz**, intente leer el código de un mando a distancia (p.ej., un control de puerta de garaje) usando la opción *Leer*. En **Infrarrojos**, haga que Flipper aprenda un botón de su mando de TV y luego pruébelo emulando ese botón.  
4. **Pruebas de alcance:** Pruebe la funcionalidad Bluetooth: conecte un altavoz Bluetooth al Flipper o use la app móvil para enviar un audio breve. Verifique también el encendido y apagado de la radio Sub-GHz midiendo el alcance máximo (FCC limita ~50 m).

## Reflexión ética

Como indica INCIBE, el uso del Flipper Zero requiere responsabilidad: no use el dispositivo para «acceso no autorizado», espionaje o daño a sistemas ajenos:contentReference[oaicite:36]{index=36}. Úselo solo con tarjetas y dispositivos propios o con permiso explícito. Por ejemplo, es **ético clonar** una tarjeta de acceso de su casa si es de su propiedad, pero no hacerlo con la tarjeta de otra persona sin autorización. Además, nunca interrumpa intencionadamente la privacidad o seguridad de terceros. Mantenga siempre el equipo bajo su control físico y evite acciones peligrosas que puedan poner en riesgo su integridad o la de otros.
