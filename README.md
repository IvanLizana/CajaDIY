# CajaDIY

**Generador de cajas paramétricas para electrónica DIY e impresión 3D** (ESP32, Arduino, Raspberry Pi…).
Por **AstroRemoto powered by FourIndustry**.

Defines las medidas interiores, la tapa, los postes de la placa, los agujeros para conectores y hasta tus logos, y CajaDIY genera los STL de la caja y la tapa listos para imprimir.

## Descargar
En **[Releases](../../releases/latest)**:
- `CajaDIY_Setup_<versión>.exe` — instalador para Windows con OpenSCAD incluido (recomendado).
- `CajaDIY_SinOpenSCAD_Setup_<versión>.exe` — instalador más liviano; usa el OpenSCAD que tengas instalado ([openscad.org](https://openscad.org/downloads.html)).

Requisitos: Windows 10/11 de 64 bits. No hace falta Python. El instalador no pide administrador.

## Qué hace
- Caja con pared, radios y pestañas de montaje (2 o 4, con avellanado y puentes para amarras).
- 8 tipos de tapa: con bisagra, a presión con broches, por fricción, con tornillos (exterior o embutida), con imanes, corredera y campana.
- Postes para la placa con plantillas (Arduino UNO, Raspberry Pi 4/5, ESP32 DevKit), tabiques interiores.
- Agujeros en las 6 caras (rectangulares con radio o circulares) con catálogo de conectores (USB-C, micro-USB, USB-A, RJ45, jack, prensaestopas PG7, M12, borneras, OLED, LED).
- Logos e imágenes en cualquier cara: en relieve, grabados o calados, varios por cara; se escalan solos.
- Vista 2D con avisos de colisiones, vista previa en OpenSCAD, exportación de STL por separado.
- Español, English, Polski, Deutsch, Français.

## Licencia
El ejecutable se distribuye bajo la licencia MIT (ver `LICENSE`). El código fuente no se publica.
Componentes de terceros incluidos y sus licencias: ver `TERCEROS.md`.
