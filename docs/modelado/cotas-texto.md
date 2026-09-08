# Cotas y anotación 3D

Estas son las anotaciones **dentro del modelo 3D**. Para las cotas sobre la hoja impresa, mira [Composición de láminas](../laminas/anotacion.md).

## Cotas

**`D`** activa Cota:

1. Clic en el primer punto (las inferencias enganchan extremos y puntos medios).
2. Clic en el segundo punto.
3. Mueve para separar la línea de cota del modelo y clic para fijarla.

La cota queda **anclada a la geometría**: muestra la distancia real y vive en 3D con el modelo. El desplegable **Estilo de cota** de la barra de herramientas controla color, altura de texto, decimales y **unidades** (metros, centímetros, pulgadas, pies, y las fraccionarias `1 1/2"` — ver [medidas por teclado](dibujo.md#medidas-por-teclado-metros-centimetros-pulgadas-pies)). Las cotas se seleccionan, se mueven con su ancla clavada, se borran con `Supr` y salen en los [marcos de las láminas](../laminas/marcos.md#extras-del-marco) si activas «Anotaciones del modelo».

## Texto guía

La herramienta **Texto** (`X`) coloca etiquetas con línea guía apuntando a una cara o arista — nombres de ambientes, notas de obra. El texto siempre mira a la cámara; se mueve con su ancla clavada, se edita con doble clic y viaja al `.skp`. Cotas y textos guía pueden vivir en una **capa**: apaga «Cotas» y desaparecen de la vista y de las láminas que no las quieren.

## Texto 3D

Dibujo ▸ **Texto 3D** genera letras con geometría real (extruibles, pintables) — para letreros y monumentos, como las letras de una plaza.

## Cinta métrica y transportador

- **Cinta** (`T`): mide y deja **guías** punteadas de construcción (líneas infinitas o puntos guía).
- **Transportador** (`H`): guías angulares.
- Las guías no son geometría: no salen en exports ni metrados, y se limpian con Edición ▸ Eliminar guías.
