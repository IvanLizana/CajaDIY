# Accesibilidad

CajaDIY quiere ser usable por la mayor cantidad de personas posible. Esto es lo que hay hoy y lo que todavía falta.

## Entornos compatibles
- Windows 10 y 11 de 64 bits.
- Interfaz en español, inglés, polaco, alemán y francés (se cambia en vivo, sin reiniciar).

## Lo que ya funciona
- Interfaz de escritorio estándar de Windows (Tkinter): respeta el tamaño de texto y la escala de pantalla del sistema.
- Todos los valores se escriben en campos de texto; no hace falta arrastrar con el mouse.
- Los avisos de diseño se muestran en texto en la barra de estado, no solo con colores.
- Manual de usuario en PDF para personas sin experiencia previa.

## Limitaciones conocidas
- El lienzo 2D (planta, frontal, lateral, isométrica) es gráfico: un lector de pantalla no puede describirlo. Las medidas y avisos sí están en los campos y en la barra de estado.
- Algunos colores del lienzo pueden ser difíciles de distinguir con daltonismo.
- No todos los controles tienen atajos de teclado.
- La vista previa 3D la muestra OpenSCAD, con su propia accesibilidad.

## Cómo reportar una barrera
Abre un issue con la plantilla **«Reportar un fallo»** y el título **«Accesibilidad: …»**. Cuenta qué intentabas hacer, qué te lo impidió y qué tecnología de apoyo usas (lector de pantalla, ampliador, solo teclado…).
