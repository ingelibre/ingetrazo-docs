# Herramientas de dibujo

Todas comparten el mismo lenguaje: clic para empezar, las **inferencias** te enganchan a la geometría existente, y el **VCB** acepta la medida exacta por teclado (escribe y Enter, sin hacer clic en ningún campo).

## Líneas y polígonos

| Herramienta | Atajo | Cómo se usa |
|---|---|---|
| **Línea** | `L` | Clic a clic; teclea la longitud para el tramo exacto. Cierra un contorno y la cara se crea sola. |
| **Rectángulo** | `R` | Dos esquinas; teclea `ancho,alto` (ej. `6,4`). |
| **Rectángulo rotado** | `K` | Primero la base (dos puntos), luego el alto. |
| **Círculo** | `C` | Centro y radio; teclea el radio. |
| **Polígono** | `G` | Centro y radio; teclea el número de lados. |

## Arcos

| Herramienta | Atajo | Cómo se usa |
|---|---|---|
| **Arco 3 puntos** | `A` | Extremo, extremo y un punto del arco. |
| **Arco por centro** | `J` | Centro, radio inicial y barrido. |
| **Arco tangente** | `O` | Continúa tangente desde el extremo de una arista. |

## Derivadas

| Herramienta | Atajo | Cómo se usa |
|---|---|---|
| **Equidistancia (Offset)** | `F` | Copia el contorno de una cara hacia adentro o afuera, a distancia exacta. El clásico para espesores de muro. |
| **Sígueme (Follow me)** | `W` | Extruye un perfil a lo largo de un camino: molduras, tuberías, sardineles. |
| **Texto 3D** | — | Dibujo ▸ Texto 3D: letras con volumen real, listas para extruir o pintar. |

### Sígueme, tres maneras

Como en SketchUp, dibuja el perfil **perpendicular al camino** (lo más fácil: sobre una cara, y borra las aristas que sobren).

1. **Arrastrar por el camino** — activa Sígueme (`W`), haz clic en el perfil y mueve el cursor por el camino tocando sus aristas: el camino se resalta en **rojo** y la extrusión se previsualiza en vivo, con sus ingletes. Clic (o soltar el botón, si arrastraste) al llegar al final; `Esc` empieza de nuevo. Si te saltas tramos de un arco, se siguen las aristas conectadas que hay en medio; si retrocedes, el camino se acorta.
2. **Camino preseleccionado** — selecciona las aristas del camino (un clic en un segmento de círculo toma todo el contorno), activa Sígueme y haz clic en el perfil: se extruye de una vez.
3. **Perímetro de una cara** — selecciona la cara cuyo borde es el camino y haz clic en el perfil; o, mientras arrastras, mantén `Alt` sobre una cara para usar su perímetro. Es el atajo para molduras alrededor de una losa y para **tornear**: un círculo como camino y medio perfil como sección.

## Medidas por teclado: metros, centímetros, pulgadas, pies

Los números sin sufijo son **metros**. Cada campo puede llevar su propia unidad, así que puedes dibujar la madera o la tubería en pulgadas y las luces en metros dentro del mismo modelo:

| Escribes | Vale |
|---|---|
| `3,2` | 3,20 m |
| `30cm` · `1500mm` | 0,30 m · 1,50 m |
| `2"` · `2in` | 2 pulgadas |
| `1'` · `1ft` | 1 pie |
| `1'6"` | 1 pie 6 pulgadas |
| `3/4"` · `1'3/4"` | fracciones de pulgada |
| `2";4"` | rectángulo de 2 × 4 pulgadas |
| `3,2;1'6";10cm` | desplazamiento X, Y, Z con unidades mezcladas |

Las comillas y la barra de fracción solo se aceptan después de un número, así que `I` y `F` siguen siendo atajos de herramienta. Las cotas del modelo pueden mostrarse en `in`, `ft` o `ft-in` desde el estilo de cotas de la bandeja.

## El plano de trabajo

Las herramientas dibujan sobre el **plano que estás mirando**: en vista superior dibujas en planta; si empiezas sobre una cara existente, dibujas sobre esa cara. El primer punto sin inferencia queda en el plano de la vista actual — así el trazo nunca "se escapa" a una profundidad inesperada.

!!! tip "Dibujar en vistas estándar"
    Para trabajo de precisión tipo 2D, combina **vista estándar + proyección paralela** (`P`): frontal para fachadas, superior para plantas. Las medidas que ves en pantalla son las reales del plano, sin efecto de perspectiva.

## Inferencias

Los puntos de colores mientras dibujas:

- **Verde** — extremo de arista.
- **Cian** — punto medio.
- **Rojo/verde/azul** — sobre un eje del sistema (X este, Y norte, Z vertical).
- **Magenta** — paralela o perpendicular a una arista existente.

Mantén el mouse un instante sobre un punto para "memorizarlo" y proyectar desde él.
