# Política de seguridad

## Versiones con soporte
Solo la última versión publicada en [Releases](../../releases/latest) recibe correcciones. Antes de reportar, comprueba que el problema sigue en esa versión.

## Cómo reportar una vulnerabilidad
**No abras un issue público.** Usa el reporte privado de GitHub:

1. Entra en la pestaña **Security** de este repositorio.
2. Pulsa **Report a vulnerability**.
3. Describe el problema, la versión afectada y, si puedes, cómo reproducirlo.

Se intentará responder dentro de una semana. Si se confirma, se publicará una versión corregida y se te dará crédito en las notas, salvo que prefieras quedar en el anonimato.

## Qué hace CajaDIY en tu equipo
Para que puedas valorar los riesgos:
- Se instala en tu carpeta de usuario y **no pide permisos de administrador**.
- **No envía datos ni busca actualizaciones**: lo único que hace con internet es abrir en tu navegador la página de descarga de OpenSCAD si tú lo pides (cuando no lo encuentra).
- Ejecuta **OpenSCAD** (instalado por ti) para generar los STL y la vista previa.
- Lee y escribe solo los archivos que tú eliges (perfiles, imágenes, `.scad`, `.stl`), su `config.json` y archivos temporales en la carpeta temporal de Windows.

Verifica siempre el instalador con el SHA-256 publicado en las notas de cada versión.
