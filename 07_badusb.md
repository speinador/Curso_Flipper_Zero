# 07_badusb.md

## Bad USB (Emulación HID)

El Flipper Zero puede actuar como un **dispositivo HID USB malicioso** (BadUSB), es decir, se conecta a un computador y se hace pasar por teclado o ratón. Al ejecutar un *payload* de BadUSB, el Flipper envía comandos de teclado preprogramados a la máquina conectada, lo cual puede abrir terminales, cambiar configuraciones o instalar software automáticamente:contentReference[oaicite:53]{index=53}. Estos payloads se escriben en formato DuckyScript (.txt) que Flipper ejecuta línea por línea, como si se escribieran en el teclado. 

El scripting de Flipper es compatible con DuckyScript 1.0 con extensiones. Por ejemplo, soporte de métodos Alt+Numpad y SysRq. Para usarlo, primero cree un archivo de texto con comandos (p.ej., `DELAY 1000`, `GUI r`, `STRING notepad`, `ENTER`, etc.) usando cualquier editor. Luego copie este archivo a la carpeta `/microSD/badusb/` del Flipper usando qFlipper o la app móvil. En el menú **Bad USB** del dispositivo aparecerá su payload. Puede ejecutar el payload en modo USB (connectores USB) o en modo BLE (Bluetooth):contentReference[oaicite:54]{index=54}. Seleccione el payload y presione *Run* para inyectar los comandos en el equipo destino.

## Laboratorio práctico

1. Conecte Flipper al PC con un cable USB-C. En la app móvil o qFlipper, diríjase a *Sistema → Flasher (o Desktop → BadUSB)*.  
2. Prepare un payload sencillo: cree un archivo `demo.txt` con contenido DuckyScript, por ejemplo:

```
DELAY 5000
GUI r
STRING notepad
ENTER
STRING HolaFlipper
ENTER
```

3. Copie `demo.txt` a la carpeta `microSD/badusb/` del Flipper usando qFlipper (o acceda a la unidad que aparece al conectar).  
4. En el menú del Flipper, vaya a **Bad USB**. Debería ver `demo.txt` listado. Selecciónelo. Asegúrese de que la aplicación BadUSB muestre el ícono de USB.  
5. Conecte el Flipper al PC y, con éste desbloqueado y listo para recibir teclazos, pulse *Run* en el Flipper. Tras unos segundos de delay, debería abrirse la ventana de ejecutar (Win+R), y luego *Notepad* con el texto “HolaFlipper” escrito automáticamente.  

> **Nota:** En modo BLE, se configuraría Flipper por Bluetooth como un teclado inalámbrico HID. El procedimiento es similar, pero requiere emparejar el Flipper como dispositivo Bluetooth HID en el sistema.

## Reflexión ética

La función BadUSB puede ser poderosa y peligrosa. Un uso indebido puede inyectar malware o comandos no autorizados en equipos ajenos:contentReference[oaicite:55]{index=55}. **Solo utilice payloads BadUSB en computadoras suyas o donde tenga permiso explícito**. Nunca conecte su Flipper como teclado a un sistema público o de terceros sin consentimiento. Además, sea cauteloso al escribir scripts: errores como bucles infinitos o comandos peligrosos pueden causar daños. Use DuckyScript con responsabilidad, y considere siempre la legislación sobre acceso y uso de sistemas informáticos antes de probar ataques de BadUSB en entornos reales.
