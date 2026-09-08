# Cotas, textos, formas y cajetín

## Cotas sobre la hoja

La herramienta **Cota** del compositor acota sobre el dibujo del marco:

1. **Clic en el primer punto** — sobre un vértice o arista del dibujo aparece el **punto verde**: el snap engancha la geometría real visible del marco.
2. **Clic en el segundo punto** (también en verde).
3. **Mueve y tercer clic** para separar la línea de cota del dibujo — con sus líneas de extensión, como manda el dibujo técnico.

### Cotas ancladas al modelo

Si ambos puntos engancharon en verde, la cota queda **anclada a los puntos 3D del modelo**:

- La etiqueta muestra la **distancia real 3D exacta** (no una medida de papel multiplicada).
- Si **editas el modelo** (la pared se estira de 6.00 a 6.20 m), la cota se mueve y **se re-mide sola**.
- Si mueves el marco, cambias su escala, su vista o su giro, la cota lo sigue.
- Al seleccionarla, sus manijas son **verdes** (ancladas) o azules (cota libre de papel). Arrastrar a mano un extremo la libera del anclaje (con deshacer).

### Estilo de cota

En sus propiedades: **separación**, **altura de texto**, **decimales**, **unidades** (m, cm, mm, pulgadas, pies, pies-pulgadas y sus fraccionarias), extremos (**trazos oblicuos**, flechas o ninguno), grosor, color, fondo del texto y texto manual si quieres reemplazar la medida. El agarre central de la línea permite reacomodar la separación cuando quieras. **El estilo de la última cota que editaste es el de las nuevas**, y se recuerda entre sesiones.

### Cotas en cadena

La herramienta **Cotas en cadena** (junto a la cota) acota varios tramos seguidos sobre **una sola línea de cota**:

1. Clic en el primer punto y en el segundo.
2. Tercer clic para fijar la separación de la línea.
3. Cada clic siguiente añade el siguiente tramo sobre la misma línea (con un quiebre, el tramo nuevo se acomoda para pasar por la línea de la cadena).
4. Clic sobre el último punto, `Esc` o cambiar de herramienta termina la cadena y apila la **cota total** una fila más afuera (con dos tramos o más; `Ctrl+Z` la quita si sobra).

Los puntos enganchados en verde anclan cada tramo al modelo, como una cota normal.

### Cota angular

La herramienta **Cota angular**: clic en el **vértice**, clic en un punto de cada lado y un cuarto clic para el **radio del arco**. Mide el ángulo real (anclada, si engancha en verde), con su arco, sus flechas y el texto alineado o recto.

## Cotas de nivel

La herramienta **Nivel** pone la marca de nivel con un clic sobre un punto de una vista: lee la **altura del punto** y escribe «N.P.T. +0.15» junto al símbolo — triángulo sobre su vértice en secciones y elevaciones, círculo en cuadrantes en plantas (el marco de planta lo elige solo). Anclada al modelo, sigue al punto si la geometría cambia y actualiza la altura; se puede deslizar por la lámina y queda una guía fina hasta el punto.

En sus propiedades: **texto** con `{z}` (o sin él: el nivel se añade al final), **nivel de referencia** (la altura del modelo que se lee como ±0.00), decimales, símbolo, tamaño, largo de la línea de nivel, lado, grosor y color. Un clic fuera de la geometría pone una cota libre con el nivel que escribas.

## Etiquetas con guía

La herramienta **Etiqueta**: clic en el punto que señalas (engancha en verde sobre el dibujo) y clic donde va el texto. La guía sigue al punto si mueves el texto; anclada a un marco, se mueve con él. Fuente, tamaño, **negrita, cursiva, subrayado**, color, fondo, punta de flecha y línea a la izquierda o a la derecha en el panel.

## Llamadas de detalle

La herramienta **Llamada** encuadra (rectángulo o círculo a trazos) la parte de una vista que otro dibujo amplía y pone la burbuja **«3 / L-05»** con una guía. La burbuja se arrastra aparte; el encuadre se mueve y redimensiona como cualquier ítem. Dibujada sobre un marco queda ligada a él y se mueve con él. Número, lámina (admite `{lamina}`), forma, tamaño, grosor y color en el panel.

## Formas

Línea, **flecha**, rectángulo (con **radio de esquinas**), elipse y **polígono regular** (3–24 lados). Cada forma con su **color de línea**, grosor, y — para las cerradas — **relleno con color propio**.

## Texto e imágenes

- **Texto**: bloques con fuente, tamaño en puntos, **negrita, cursiva y subrayado**, color, fondo y alineación. **Doble clic** lo edita **en su sitio**, con la misma letra al mismo tamaño; clic fuera o `Ctrl+Enter` confirma, `Esc` cancela. Un texto puede quedar **ligado a un marco** («se mueve con su marco») y usar campos: `{escala}` lee la escala de ese marco, `{lamina}` y `{proyecto}` el cajetín, `{fecha}` la fecha. **Añadir etiqueta de escala** en el panel del marco pone un texto así, ya escrito.
- **Imagen**: logos, fotos de obra, vistas auxiliares (PNG/JPG). Con **opacidad**, **forma del recorte** (rectángulo, esquinas redondeadas, elipse o círculo), **borde desvanecido** en milímetros, **ajuste** (estirar, cubrir recortando o contener entera) y contorno opcional — una foto en círculo fundida al papel, como en las láminas de presentación.
- **Perfil de terreno**: la herramienta **Perfil** dibuja el perfil longitudinal de un [trazado](../terreno/rutas-perfil.md) sobre la lámina, con escala horizontal y vertical, exageración vertical, progresivas y cotas; muestreado del levantamiento de dron o del DEM, y se actualiza si el trazado cambia.

## Cajetín

El membrete del plano — **el** ítem de una lámina:

- **Campos editables**: la tabla de propiedades permite renombrar, **agregar y quitar filas** (PROYECTO, AUTOR, FECHA, ESCALA, LÁMINA, y los que tu expediente pida: DISTRITO, REGIÓN…). Los valores admiten campos: `{fecha}`, `{lamina}`, `{total}`…
- **1 a 4 columnas** de campos, lado a lado, como los cajetines anchos reales.
- **Diseño**: siete presets de aspecto —esquinas cuadradas, redondeadas o achaflanadas; cuadrícula, banda de cabecera o minimalista; doble borde, relleno de rótulos, colores— que cambian **cómo se ve**, nunca las filas ni el tamaño. Cada detalle es editable aparte: grosores del borde exterior y de las líneas interiores, ancho de la columna de rótulos, colores de rótulo, texto y línea.
- **Plantillas de cajetín** (botón **Plantillas…**): guarda el tuyo —filas, tamaño y aspecto— con nombre, aplícalo a otra lámina y márcalo como **predeterminado**: cada cajetín nuevo nace de él. **Copiar estilo / Pegar estilo** también funciona entre cajetines.
- **Las filas se reparten el alto según lo que llevan**: un nombre de proyecto largo baja a dos o tres líneas y su fila crece —hasta tres veces su parte— a costa de las filas que no usaban la suya, así todos los valores salen del mismo tamaño; solo si aun así no cabe, la letra se condensa.

## Escala gráfica, norte y leyenda

- **Escala gráfica**: la barra de segmentos blanco/negro con metros — el lector mide incluso sobre una fotocopia. Sigue la escala que le indiques.
- **Flecha de norte**: rotable al norte de tu proyecto.
- **Leyenda de capas**: lista las capas visibles del modelo, con refresco manual.
