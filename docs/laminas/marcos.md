# Marcos de vista y escala

Un **marco de vista** es una ventana al modelo colocada sobre la hoja. Es el item central del compositor.

## Crear un marco

Con la herramienta **Marco** dibuja el rectángulo sobre la hoja (dos clics o arrastre). En sus propiedades eliges:

- **Vista**: la cámara actual, una **vista estándar** (planta, frontal, laterales, isométrica…) o cualquiera de tus **escenas guardadas** — una escena "Planta primer piso" con sus capas configuradas es tu plano listo.
- **Escala 1:N**: la ecuación sagrada del compositor — *1:100 en un marco de 200 mm de alto muestra exactamente 20 m de modelo*. Siempre, sin aproximaciones. Cambias la escala y el contenido se reencuadra exacto.
- **Tamaño del marco** en mm, por arrastre o numérico.

## Estilos de render

| Estilo | Qué muestra |
|---|---|
| **Estilo del modelo** | El modelo tal como se ve en el visor: materiales, texturas, sombreado. |
| **Estilos guardados** | Cualquier estilo de la biblioteca (Líneas ocultas, Arquitectónico, los tuyos…), por marco, como los viewports de LayOut. |
| **Vector (líneas ocultas)** | El dibujo que entintaría un dibujante: las **líneas ocultas se eliminan con cálculo exacto**, en vectores reales para el PDF y el DXF. |

### Plumas y poché del estilo Vector

El estilo Vector clasifica cada trazo y lo dibuja con su pluma, como un plano de oficina:

| Clase | Pluma por defecto | Qué es |
|---|---|---|
| **Corte de sección** | 0,50 mm | Donde el plano de sección atraviesa un sólido. |
| **Perfiles** | 0,35 mm | Siluetas y contornos contra el fondo — los *Profiles* de SketchUp. |
| **Aristas** | 0,18 mm | Las demás aristas, entre dos caras visibles. |

Donde la sección corta un **sólido cerrado**, el marco rellena el corte (el *poché*): **sólido** o **achurado a 45°**, con color y paso de achurado a tu gusto; una superficie abierta queda en blanco. Las plumas y el relleno se ajustan en la sección **Plumas del vectorial** del panel, que solo aparece con este estilo. La exportación DXF reparte las clases en capas `VISTA`, `VISTA-PERFIL` y `VISTA-CORTE` para la tabla de plumas de tu CAD.

## Rótulo de vista

Marca **Rótulo de vista** en el panel del marco y elige el estilo:

- **Numerado, con línea debajo** (LayOut): burbuja con el **número** de la vista arriba y la **lámina** abajo, título en negrita, «ESC. 1:N» y una línea de base hasta el borde del marco. Con subtítulo opcional («N.P.T. +0.15»).
- **Barra vertical**: una franja a la izquierda del marco con título, subtítulo y escala girados 90°, y la burbuja al pie — el hábito de los planos brasileños.
- **Línea simple**: la línea centrada de siempre.

Título, subtítulo, número y lámina admiten campos dinámicos: `{lamina}` lee el cajetín, `{escala}` la escala de ese marco, `{escena}` el nombre de la escena. Alineación, posición (debajo o encima) y tamaño del texto en el mismo panel. Todo se edita en vivo, sin recalcular la vista.

## Marcas de sección

Marca **Marcas de sección (A–A)** y el marco dibuja la traza de cada plano de sección del modelo que atraviesa su vista: la línea de corte a raya y punto, las flechas hacia el lado que mira la sección y la **letra del plano** en burbujas a ambos extremos. Así la planta dice por dónde va el «Corte A-A». La letra es el símbolo del plano (Ventana ▸ Secciones); sin símbolo, A, B, C… por orden. Un plano paralelo a la vista no deja marca.

## Extras del marco

- **Anotaciones del modelo**: las cotas y textos con guía dibujados en el modelador salen en el marco, con la altura de texto que elijas.
- **Cuadrícula de coordenadas**: el grid en metros de modelo sobre la vista (el hábito de los planos con malla), con el paso que elijas.
- **Refrescar**: re-renderiza el marco desde el modelo actual — los marcos no son capturas, son ventanas vivas.

!!! tip "El flujo recomendado"
    Prepara **escenas** en el modelador (planta con las capas correctas, elevaciones frontales) y en el compositor solo colócalas a escala. Cuando el proyecto cambie, las láminas se actualizan solas.
