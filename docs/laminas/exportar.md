# Exportar PDF y DXF

## Vista previa de impresión

**Vista previa de impresión…** muestra la lámina tal como saldrá: tamaño real, grosores de línea, sin manijas ni imanes. Es el lugar para revisar antes de exportar.

## PDF de una lámina

**Exportar PDF…** escribe la lámina actual con métrica física exacta: el A3 sale A3, la escala 1:100 **mide** 1:100 sobre el papel impreso. El PDF es **vectorial** — las líneas del estilo Vectorial son curvas reales con sus tres plumas y su poché, no píxeles: se imprime nítido a cualquier tamaño. Nada de la pantalla se cuela: ni la selección del modelo, ni las manijas, ni los imanes.

## El atlas: todas las láminas en un PDF

**Exportar todas las láminas (PDF)…** genera un solo archivo con cada lámina del documento en su propia página (cada una con su tamaño de papel) — el juego de planos completo del expediente en un clic.

## DXF hacia IngeCAD / AutoCAD

Con un marco seleccionado, **Exportar vista como DXF…** escribe el dibujo vectorial de esa vista (las líneas visibles exactas, en metros de modelo, con el giro de la vista aplicado) como DXF R12 — lo abre [IngeCAD](https://ingecad.org), AutoCAD, LibreCAD o QGIS. Las clases de línea van en capas separadas —`VISTA`, `VISTA-PERFIL`, `VISTA-CORTE`— para tu tabla de plumas. Es el puente para quien remata detalles 2D en su CAD de siempre.

!!! tip "Antes de exportar"
    - **Actualiza los marcos** si editaste el modelo con el compositor abierto (o deja el renderizado automático encendido).
    - Revisa a **zoom 100 %** (tamaño real del papel) o en la vista previa: los grosores de línea y tamaños de texto se ven exactamente como saldrán impresos.
    - Los tres [ejemplos](../primeros-pasos/ejemplos.md) con lámina traen el PDF resultante al lado, por si quieres comparar.
