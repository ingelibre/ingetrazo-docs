# Cotas, formas y cajetín

## Cotas sobre la hoja

La herramienta **Cota** del compositor acota sobre el dibujo del marco:

1. **Clic en el primer punto** — sobre un vértice o arista del dibujo aparece el **punto verde**: el snap engancha la geometría real visible del marco.
2. **Clic en el segundo punto** (también en verde).
3. **Mueve y tercer clic** para separar la línea de cota del dibujo — con sus líneas de extensión, como manda el dibujo técnico.

### Cotas ancladas al modelo

Si ambos puntos engancharon en verde, la cota queda **anclada a los puntos 3D del modelo**:

- La etiqueta muestra la **distancia real 3D exacta** (no una medida de papel multiplicada).
- Si **editas el modelo** (la pared se estira de 6.00 a 6.20 m), la cota se mueve y **se re-mide sola**.
- Si mueves el marco, cambias su escala o su vista, la cota lo sigue.
- Al seleccionarla, sus manijas son **verdes** (ancladas) o azules (cota libre de papel). Arrastrar a mano un extremo la libera del anclaje (con deshacer).

### Estilo de cota

En sus propiedades: **separación**, **altura de texto**, **decimales**, extremos (**trazos oblicuos**, flechas o ninguno), grosor, color, y texto manual si quieres reemplazar la medida. El agarre central de la línea permite reacomodar la separación cuando quieras.

### Cotas en cadena

La herramienta **Cotas en cadena** (junto a la cota) acota varios tramos seguidos sobre **una sola línea de cota**:

1. Clic en el primer punto y en el segundo.
2. Tercer clic para fijar la separación de la línea.
3. Cada clic siguiente añade el siguiente tramo sobre la misma línea (con un quiebre, el tramo nuevo se acomoda para pasar por la línea de la cadena).
4. Clic sobre el último punto, `Esc` o cambiar de herramienta termina la cadena y apila la **cota total** una fila más afuera (con dos tramos o más; `Ctrl+Z` la quita si sobra).

Los puntos enganchados en verde anclan cada tramo al modelo, como una cota normal. El estilo de la última cota editada es el de las nuevas, y se recuerda entre sesiones.

## Cotas de nivel

La herramienta **Nivel** pone la marca de nivel con un clic sobre un punto de una vista: lee la **altura del punto** y escribe «N.P.T. +0.15» junto al símbolo — triángulo sobre su vértice en secciones y elevaciones, círculo en cuadrantes en plantas (el marco de planta lo elige solo). Anclada al modelo, sigue al punto si la geometría cambia y actualiza la altura; se puede deslizar por la lámina y queda una guía fina hasta el punto.

En sus propiedades: **texto** con `{z}` (o sin él: el nivel se añade al final), **nivel de referencia** (la altura del modelo que se lee como ±0.00), decimales, símbolo, tamaño, largo de la línea de nivel, lado, grosor y color. Un clic fuera de la geometría pone una cota libre con el nivel que escribas.

## Llamadas de detalle

La herramienta **Llamada** encuadra (rectángulo o círculo a trazos) la parte de una vista que otro dibujo amplía y pone la burbuja **«3 / L-05»** con una guía. La burbuja se arrastra aparte; el encuadre se mueve y redimensiona como cualquier ítem. Dibujada sobre un marco queda ligada a él y se mueve con él. Número, lámina (admite `{lamina}`), forma, tamaño, grosor y color en el panel.

## Formas

Línea, **flecha**, rectángulo (con **radio de esquinas**), elipse y **polígono regular** (3–24 lados). Cada forma con su **color de línea**, grosor, y — para las cerradas — **relleno con color propio**.

## Texto e imágenes

- **Texto**: bloques con fuente, tamaño en puntos, negrita/cursiva, color y alineación.
- **Imagen**: logos, fotos de obra, vistas auxiliares (PNG/JPG). Con **opacidad**, **forma del recorte** (rectángulo, esquinas redondeadas, elipse o círculo), **borde desvanecido** en milímetros, **ajuste** (estirar, cubrir recortando o contener entera) y contorno opcional — una foto en círculo fundida al papel, como en las láminas de presentación.

## Cajetín

El membrete del plano — **el** item de una lámina:

- **Campos editables**: la tabla de propiedades permite renombrar, **agregar y quitar filas** (PROYECTO, AUTOR, FECHA, ESCALA, LÁMINA, y los que tu expediente pida: DISTRITO, REGIÓN…).
- **1 a 4 columnas** de campos, lado a lado, como los cajetines anchos reales.
- **Grosores** independientes para el borde exterior y las líneas interiores; ancho y alto exactos en mm.
- Los textos largos (el nombre completo del proyecto) **bajan a dos o tres líneas** dentro de su celda y solo si aun así no caben, la letra se condensa.

## Escala gráfica, norte y leyenda

- **Escala gráfica**: la barra de segmentos blanco/negro con metros — el lector mide incluso sobre una fotocopia. Sigue la escala que le indiques.
- **Flecha de norte**: rotable al norte de tu proyecto.
- **Leyenda de capas**: lista las capas visibles del modelo, con refresco manual.
