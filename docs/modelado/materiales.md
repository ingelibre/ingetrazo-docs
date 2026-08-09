# Materiales y texturas

## Pintar

**`B`** abre la herramienta Pintar y el panel de **Materiales** de la bandeja:

- Elige un **color** o una **textura** y haz clic sobre caras (o sobre grupos enteros).
- **Gotero**: con `Alt`, el clic *toma* el material de la cara bajo el cursor en lugar de pintarla.
- **+ Color…** y **+ Textura…** crean materiales propios; puedes traer cualquier imagen PNG/JPG como textura.

## Texturas

- La proyección es **compatible con SketchUp**: planar por cara, con UVs que sobreviven el viaje de ida y vuelta por `.skp`.
- Las texturas **viajan dentro del documento** `.igz`: el archivo es autocontenido, lo llevas a otra PC y abre completo.
- Los materiales **translúcidos** (vidrio) y las texturas **caladas** (mallas, celosías) se ven correctamente en el viewport.

## Caras

- Cada cara tiene **frente y dorso** (el dorso se dibuja azul grisáceo). **Invertir caras** (clic derecho) las voltea — importa para texturizar y para exportar.
- **Aristas suaves**: las superficies curvas (cilindros, arcos extruidos) se muestran continuas; sus aristas de control son "soft" y no ensucian el dibujo.

!!! tip "Limpieza de la caché de texturas"
    Las imágenes que llegan de archivos `.skp` importados se guardan en una caché del programa (nunca junto a tus archivos). Archivo ▸ Importar ▸ Limpiar caché de texturas importadas… la vacía si necesitas espacio.
