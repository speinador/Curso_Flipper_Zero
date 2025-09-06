# 06_infrarrojos.md

## Infrarrojos (IR)

El Flipper Zero dispone de un módulo de infrarrojos integrado (ventana plástica IR transparente, 3 LEDs IR emisores y un receptor IR):contentReference[oaicite:51]{index=51}. Esto le permite **leer y emular señales IR** de mandos a distancia de TVs, aires acondicionados y otros equipos electrónicos. En el menú **Infrarrojos**, puede utilizar *Aprender nuevo mando* para capturar cada botón de un mando tradicional: cada señal se guarda por separado. Luego puede reproducir esas señales desde *Guardados* para controlar el dispositivo original. 

![plot](https://github.com/speinador/Curso_Flipper_Zero/blob/main/img/Infrarrojos.png)

Adicionalmente, el Flipper ofrece la función *Mando universal*: al seleccionar esta opción envía automáticamente señales de un diccionario de protocolos IR conocidos (almacenado en la SD) de manera secuencial (equivale a un ataque de fuerza bruta de mandos IR):contentReference[oaicite:52]{index=52}. Esto puede encender/apagar TVs o cambiar canales simplemente probando múltiples códigos. También hay ajustes avanzados, como configurar salidas GPIO para conectar un transmisor IR externo al dispositivo. 

## Laboratorio práctico

1. Encienda el Flipper y vaya al menú **Infrarrojos**. Seleccione *Aprender mando*.  
2. Tome un mando a distancia (p.ej., de un televisor) y presione uno de sus botones mientras sostiene el Flipper enfrente. El Flipper mostrará «Signal received» cuando capture la señal. Repita esto para otros botones (p. ej., *Power*, *Vol+*, *Canal+*).  
3. Vaya a *Guardados* en el menú Infrarrojos. Seleccione el comando grabado (p. ej., “Power”) y pulse *Reproducir*. Apunte el Flipper hacia el televisor original: éste debería responder (encendiendo o apagando la señal).  
4. Experimente con *Mando universal*: seleccione esta opción y el Flipper empezará a emitir secuencialmente señales para varios modelos de TV. Observe en el televisor si enciende o apaga con alguna de ellas (puede tardar unos segundos en cada código).  
5. Si dispone de un LED IR externo o de otros módulos en GPIO, conecte un transmisor IR a los pines GPIO1-3V y use la opción *Transmisor externo* (configuración en el menú).

## Reflexión ética

El control infrarrojo es generalmente inofensivo, pero evite interferir con dispositivos de terceros sin permiso. Por ejemplo, no use el Flipper para encender/apagar TVs u otros aparatos en espacios públicos o de desconocidos. Aunque es seguro desde el punto de vista digital, manipular dispositivos ajenos sin autorización podría considerarse una molestia o invasión de privacidad. Use IR solo con equipos propios o en entornos donde no cause perjuicio. No intente desbloquear funciones protegidas de dispositivos IR comerciales (p. ej., aires acondicionados con contraseñas ocultas).
