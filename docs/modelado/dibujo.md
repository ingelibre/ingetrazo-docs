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
