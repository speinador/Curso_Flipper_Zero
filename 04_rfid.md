# 04_rfid.md

## RFID 125 kHz

Flipper Zero dispone de un módulo RFID de baja frecuencia (125 kHz) con antena incorporada en la parte trasera. Este módulo puede **leer, guardar, emular y escribir tarjetas RFID** de 125 kHz (por ejemplo EM4100, HID Prox, T5577, etc.):contentReference[oaicite:42]{index=42}. Las tarjetas LF de 125 kHz se usan habitualmente en controles de acceso (identificación de empleados, guardias, parkings) y en chips de mascotas o logística. A diferencia de NFC, estas tarjetas de 125 kHz suelen tener menor seguridad criptográfica:contentReference[oaicite:43]{index=43}. Flipper permite, por ejemplo, copiar el ID de una tarjeta (EM4100) y emularla, o clonar una tarjeta T5577 regrabable.

![plot](https://github.com/speinador/Curso_Flipper_Zero/blob/main/img/RFID.png)

En la app 125 kHz RFID del Flipper, seleccione **Leer** y acerque la tarjeta LF al dispositivo. Flipper alterna automáticamente entre ASK y PSK cada 3 segundos para intentar leer los datos:contentReference[oaicite:44]{index=44}. Cuando termine, se mostrará el ID de la tarjeta. Elija *Más → Guardar* para almacenarla. Para emular una tarjeta guardada, vaya a *Guardadas*, seleccione la tarjeta y pulse *Emular* (sostenga el Flipper con la parte trasera hacia el lector). Flipper también permite leer con codificación preseleccionada (ASK/PSK fijo) o generar tarjetas virtuales ingresando manualmente un ID (Add Manually). Además, se puede escribir datos en tarjetas T5577 regrabables con la opción correspondiente.

## Laboratorio práctico

1. Encienda el Flipper Zero y vaya al menú **125 kHz RFID**. Inserte una tarjeta o llavero RFID de 125 kHz propio (p.ej., la del acceso de su casa) cerca de la parte trasera del dispositivo y seleccione *Leer*.  
2. Espere hasta que aparezca “Capture OK” o muestre el número de ID de la tarjeta en pantalla.  
3. Pulse *Más* y luego *Guardar* para almacenar la tarjeta. Asígnela un nombre reconocible (p.ej., “Acceso Casa”).  
4. En el menú principal 125 kHz, seleccione *Guardadas* y elija la tarjeta guardada. Pulse *Emular* y acerque el Flipper al lector de puerta. Verifique que el control reprodujo correctamente la señal (p. ej., la puerta se abre).  
5. (Opcional) Si dispone de una tarjeta T5577 regrabable, use la opción *Escribir datos* para clonar el ID guardado en esa tarjeta física usando el Flipper.

## Reflexión ética

La tecnología RFID de 125 kHz se usa para acceso físico seguro, por lo que su mal uso puede comprometer la seguridad de personas o instalaciones. **Solo debe leer o clonar tarjetas propias o con autorización**. Hacerlo con tarjetas ajenas puede suponer «acceso no autorizado» a propiedades ajenas y es ilegal:contentReference[oaicite:45]{index=45}. Además, el Flipper puede emular tarjetas, pero nunca se debe utilizar para ingresar a lugares privados sin permiso. Si realiza prácticas de seguridad, hágalo en entornos controlados (p.ej., su hogar o laboratorio) y no modifique tarjetas de usuarios sin consentimiento. En cualquier caso, respete la privacidad y los sistemas de terceros al emplear el módulo RFID.
Clonar tarjetas sin autorización representa...
