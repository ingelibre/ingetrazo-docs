# Composición de láminas

El **compositor de láminas** convierte tu modelo en planos impresos sin salir de IngeTrazo — al estilo del compositor de QGIS o de LayOut: colocas **vistas del modelo a escala exacta** sobre una hoja, las acotas, les pones cajetín, y exportas PDF vectorial.

Se abre desde las **pestañas de la barra de estado** (Modelo | Lámina 1 | … | `+`) — un clic en una lámina la abre; `+` crea una nueva; **Modelo** vuelve al modelador — o desde **Archivo ▸ Compositor de láminas…**.

![Una lámina A3 exportada por IngeTrazo: planta y elevaciones a 1:100, cajetín y escala gráfica.](../images/laminas.jpeg)


## La ventana

- **Lienzo central**: la hoja, con sombra y márgenes. Zoom con `Ctrl+rueda` o con el combo de la barra de estado (*Ajustar a hoja*, *Ajustar a anchura*, porcentajes — 100 % es el **tamaño real del papel** en tu pantalla). **Desplazar** con la rueda, con el botón central o con la herramienta Mano, a cualquier zoom: la hoja nunca se te pierde (una franja queda siempre a la vista).
- **Barra de herramientas izquierda**: seleccionar, mano, pincel de formato, marco de vista, texto, etiqueta con guía, nivel, llamada de detalle, imagen, cajetín, escala gráfica, norte, leyenda, perfil de terreno, línea, flecha, rectángulo, elipse, polígono, cota, cotas en cadena y cota angular.
- **Panel derecho** (redimensionable, cabe en ~480 px): gestor de láminas, lista de **Elementos** y propiedades del ítem seleccionado. Las secciones que no usas se pliegan.
- **Barra de estado**: las mismas pestañas Modelo | Láminas, las coordenadas en mm y el zoom.

## Hojas

- Tamaños **A4 a A0**, horizontal o vertical, con margen configurable y **borde de la lámina** opcional (simple o doble, grosor y color; sale impreso).
- **Varias láminas por documento**: `+` crea, `⧉` duplica (hereda cajetín y márgenes — ideal para mantener el estilo del expediente), `−` elimina, y *Renumerar láminas* actualiza los L-01, L-02… de los cajetines.
- **Plantillas de lámina** (botón **Plantillas…**): guarda una lámina —hoja, márgenes, borde, cajetín, marcos vacíos— como plantilla con nombre; crea láminas nuevas desde ella y fija una **por defecto** para todo documento nuevo. Las plantillas son archivos en tu carpeta de usuario (*Abrir la carpeta de plantillas*): se comparten copiándolas.
- Todo se guarda **dentro del `.igz`**, con su propio deshacer. Compones una vez; cada revisión del modelo es reabrir y re-exportar — o dejar el **renderizado automático** encendido y verla actualizarse.

## Los ítems

Cada cosa sobre la hoja es un ítem: se mueve arrastrando (con imanes a márgenes, centro y otros ítems), se redimensiona por la esquina (el cursor lo indica), y tiene sus propiedades en el panel. **Doble clic** sobre un texto lo edita en su sitio; sobre un marco entra a editar la vista.

**Seleccionar varios**: arrastra un cuadro desde la hoja vacía — de izquierda a derecha selecciona lo que queda **encerrado** (azul), de derecha a izquierda lo que **toca** (verde a trazos); `Mayús` alterna, `Ctrl` añade, `Mayús+Ctrl` quita. Un clic en la hoja vacía deselecciona.

Con **clic derecho** sobre cualquier ítem:

- **Traer al frente / Subir / Bajar / Enviar al fondo** — el orden de apilado (dibuja un rectángulo de fondo, mándalo atrás, y pon todo encima).
- **Bloquear** (`Ctrl+L`) — el ítem queda visible pero **fuera del alcance del mouse**: ni clic ni cuadro lo toman, así las cotas y textos sobre un marco bloqueado se editan sin pescar el marco. La única puerta es la lista **Elementos** del panel: desde ahí se selecciona, se edita y se desbloquea. El candado lo marca.
- **Organizar** — alinear y distribuir la selección (dos o más ítems), **agrupar y desagrupar** (`Ctrl+G`, `Ctrl+Mayús+G`; un grupo se arrastra junto), **duplicar** (`Ctrl+D`). La barra «Organizar» con estos botones está oculta por defecto; clic derecho sobre la barra de herramientas para mostrarla.
- **Copiar estilo / Pegar estilo** (`Ctrl+Mayús+C` / `Ctrl+Mayús+V`) entre ítems del mismo tipo — y el **Pincel de formato** de la barra: clic en el ítem modelo, clic en los destinos, `Esc`.

**Portapapeles**: `Ctrl+C`, `Ctrl+X`, `Ctrl+V` copian ítems dentro de una lámina (el pegado cae 5 mm más abajo y a la derecha) o **entre láminas** (cae en el mismo sitio). Los textos ligados y las cotas ancladas a un marco copiado siguen al marco pegado.

Sigue con **[Marcos de vista y escala](marcos.md)** — el corazón del compositor.
