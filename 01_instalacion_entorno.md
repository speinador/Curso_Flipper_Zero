# 01_instalacion_entorno.md

## Instalación del entorno

Para comenzar a usar Flipper Zero, lo primero es preparar el entorno. Se recomienda formatear e insertar una tarjeta **MicroSD** (idealmente de 16–32 GB, hasta 256 GB) en el dispositivo, ya que Flipper almacena en ella datos como claves, tarjetas y remotos:contentReference[oaicite:22]{index=22}. A continuación, instale la **aplicación Flipper Mobile** (iOS/Android) para poder actualizar el firmware vía Bluetooth, y el software de escritorio **qFlipper** (Windows/Mac/Linux) para actualizaciones por USB:contentReference[oaicite:23]{index=23}:contentReference[oaicite:24]{index=24}. Ambos procesos permiten instalar la última versión del firmware oficial, lo cual es crucial para la seguridad y el funcionamiento óptimo del dispositivo:contentReference[oaicite:25]{index=25}:contentReference[oaicite:26]{index=26}.

Una vez que el Flipper está cargado y conectado, enciéndalo manteniendo presionado el botón %back% durante unos segundos (ver el manual si es la primera vez). Luego, en la aplicación móvil active Bluetooth en el Flipper (Menú Principal → Ajustes → Bluetooth → ON) y conéctelo con la app del teléfono. El propio app mostrará un botón de **actualizar firmware** que permitirá descargar e instalar la última versión automáticamente:contentReference[oaicite:27]{index=27}. Alternativamente, en el PC ejecute qFlipper, conecte el Flipper por cable USB-C y en la pestaña de actualización haga clic en «Instalar» o «Actualizar» para aplicar el firmware más reciente:contentReference[oaicite:28]{index=28}. 

Finalmente, configure las preferencias básicas: ajuste la hora, idioma, formato (Menú Principal → Ajustes → Sistema) y cualquier otro parámetro de usuario. Compruebe también que la tarjeta MicroSD esté formateada en FAT32 y reconocida por Flipper:contentReference[oaicite:29]{index=29}.

## Laboratorio práctico

1. Inserte una tarjeta MicroSD formateada en FAT32 en el compartimento trasero del Flipper Zero.  
2. Encienda el Flipper manteniendo pulsado el botón %back% (atras) durante 3 segundos.  
3. Instale la aplicación **Flipper Mobile** en su smartphone y siga el proceso de emparejamiento Bluetooth (Menú Principal → Ajustes → Bluetooth → ON).  
4. Con el Flipper conectado al teléfono, utilice la opción de **Actualizar** en la app móvil para instalar la versión más reciente del firmware.  
5. Descargue e instale **qFlipper Desktop** desde la página oficial. Conecte el Flipper al ordenador por USB y abra qFlipper. En la sección de actualización, haga clic en **Actualizar** para instalar el firmware.  
6. Verifique que el firmware se ha instalado correctamente viendo la versión en el menú Principal del dispositivo (Menú Principal → Ajustes → Acerca de).

## Reflexión ética

Al configurar el Flipper Zero, es vital utilizar software oficial y mantener el dispositivo actualizado:contentReference[oaicite:30]{index=30}. Descargar firmware de fuentes no autorizadas o desactualizado puede introducir **vulnerabilidades** o software malicioso. Además, considere la seguridad de sus datos: nunca deje la tarjeta MicroSD con información sensible sin cifrar, y no pierda el control físico del dispositivo. Según INCIBE, mantener el firmware al día ayuda a proteger contra amenazas conocidas:contentReference[oaicite:31]{index=31}, garantizando un uso responsable y seguro del Flipper Zero.
