# Preguntas frecuentes

## ¿Es gratis de verdad?

Sí. IngeTrazo es **software libre bajo GPL-3.0**: gratis hoy y para siempre, con el código publicado en GitHub. Sin cuentas, sin suscripciones, sin funciones bloqueadas.

## ¿Funciona sin internet?

Sí — todo el modelador, el BIM y el compositor de láminas funcionan **offline**. Solo el mapa satelital y el terreno 3D descargan imágenes mientras los usas; tu levantamiento de dron, una vez importado, también funciona sin conexión.

## ¿Puedo abrir mis `.skp` de SketchUp?

Sí, directamente y **sin conversores**: el importador nativo lee archivos de todas las versiones de SketchUp con geometría, grupos, componentes, materiales, texturas, capas, escenas y cotas. Ver [Importar y exportar](importar-exportar.md).

## ¿Mis archivos quedan atrapados en un formato propietario?

No. El `.igz` es un formato **abierto y documentado** (JSON / ZIP). Aunque IngeTrazo desapareciera mañana, tus modelos seguirían siendo legibles. Además exportas a IFC, OBJ, STL, glTF, DAE y DXF cuando quieras.

## ¿Por qué el programa rechaza a veces un empuje/tirar?

Porque esa operación habría dejado un sólido roto (no hermético). IngeTrazo prefiere **negarse a corromper el modelo**: reintenta el empuje desde otra cara o revisa si hay geometría superpuesta. Esa garantía es la que hace confiables los metrados y el STL de impresión.

## ¿La cota de mi lámina cambió sola, ¿por qué?

Porque está **anclada al modelo** y el modelo cambió — la cota siguió al vértice y se re-midió: es su trabajo. Si quieres una cota fija de papel, arrastra uno de sus extremos (se libera del anclaje) o dibújala sin engancharla en los puntos verdes.

## ¿Qué precisión tiene el terreno y el levantamiento de dron?

El terreno 3D satelital usa un DEM global (~30 m de resolución) — perfecto para contexto. Tu **levantamiento de dron** tiene la precisión de tu vuelo (centimétrica en planta con buen procesamiento). Sin puntos de control, la altitud del dron es GNSS y puede diferir del nivel del mar unos metros — IngeTrazo lo anota en los perfiles exportados.

## ¿Corre en mi máquina?

IngeTrazo pide OpenGL 3.3 (cualquier gráfica de la última década) y funciona especialmente bien en Linux — también Windows y macOS. Modelos reales de cientos de miles de triángulos orbitan a 60 fps.

## ¿Cómo reporto un problema?

En [GitHub](https://github.com/ingelibre/ingetrazo/issues), idealmente con el archivo que lo reproduce (`.igz` o `.skp`). Los archivos de ejemplo de los usuarios son la principal fuente de mejoras del importador.
