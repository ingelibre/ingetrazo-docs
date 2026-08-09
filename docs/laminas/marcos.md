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
| **Sombreado** | El modelo como en el viewport: materiales, texturas, sombreado. |
| **Técnico** | Caras blancas + aristas oscuras — el look del plano de obra. Las **líneas ocultas se eliminan con cálculo exacto** (no aproximado): el dibujo que entintaría un dibujante. |
| **Líneas** | Solo las aristas visibles. |

## Extras del marco

- **Título automático**: «Planta — 1:100» bajo el marco, con un clic.
- **Cuadrícula de coordenadas**: el grid en metros de modelo sobre la vista (el hábito de los planos con malla), con el paso que elijas.
- **Refrescar**: re-renderiza el marco desde el modelo actual — los marcos no son capturas, son ventanas vivas.

!!! tip "El flujo recomendado"
    Prepara **escenas** en el modelador (planta con las capas correctas, elevaciones frontales) y en el compositor solo colócalas a escala. Cuando el proyecto cambie, las láminas se actualizan solas.
