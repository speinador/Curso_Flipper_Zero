# 📲 NFC

## Introducción
Flipper Zero también cubre alta frecuencia (HF) 13.56 MHz, compatible con NFC y etiquetas de tarjetas de transporte o acceso moderno. Internamente lleva un lector NFC capaz de manejar MIFARE Classic (1K, 4K), NTAG, Ultralight, Felica, ICODE SLIX y otros estándares NFC≠HF. El uso es similar al RFID: en el menú NFC > Leer, Flipper mostrará qué tipo de tarjeta detecta y leerá los datos disponibles.

Por ejemplo, con una tarjeta MIFARE Classic (1K), Flipper buscará entre las claves maestras predefinidas en su diccionario interno (llaves “famosas”) para descifrarla. Si tiene éxito, mostrará los datos almacenados en sectores (p.ej. número de tarjeta, historial, etc.). Si no, solo captura el UID. Tras leerla, puedes usar Emular tarjeta o Escribir en una tarjeta compatible (por ejemplo duplicando la información a otra MIFARE UltraLight).

**Laboratorio NFC:** Toma una etiqueta/tag NFC (propia). Ve a NFC > Leer y captura su información. Observa si Flipper identifica el tipo (Classic, NTAG, etc.). Intenta escribir algunos datos simples en un tag NTAG repuestos. En Extra acciones > Mifare Classic Keys verifica las claves cargadas. Con Flipper puedes explorar la seguridad: por ejemplo, extrae las claves de una MIFARE Classic de prueba (si están en su diccionario) y repasa cómo se organizan las tarjetas. Nota: no uses tarjetas de pago o privadas reales sin permiso.

---
## 🧪 Laboratorio
1. Escanea una tarjeta de transporte...

---
## 🤔 Reflexión Ética
El acceso no autorizado a tarjetas NFC...
