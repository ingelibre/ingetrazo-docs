# Editar la geometría

## Empujar / Tirar

**`U`** — la herramienta que convierte dibujos en volúmenes. Clic sobre una cara, mueve, teclea la distancia y Enter.

- Sobre una cara de un sólido: lo **engrosa o adelgaza**.
- Sobre un dibujo dentro de una cara: **abre un vano** al llegar a la cara opuesta.
- IngeTrazo verifica cada empuje: si la operación fuera a dejar un sólido roto, la **rechaza** con un aviso — nunca corrompe el modelo.

## Mover, Rotar, Escalar

| Herramienta | Atajo | Notas |
|---|---|---|
| **Mover** | `M` | Selecciona y arrastra; teclea la distancia. Mueve puntos, aristas, caras o selecciones completas. |
| **Rotar** | `Q` | Define el plano de giro, el punto de pivote y el ángulo (o teclealo). |
| **Escalar** | `S` | Manijas en las esquinas; teclea el factor. |

## Seleccionar

**Espacio** activa Selección. Clic simple selecciona; doble clic sobre una cara toma la cara y sus aristas; arrastre dibuja ventana de selección (izquierda→derecha: solo lo contenido; derecha→izquierda: todo lo tocado). `Esc` deselecciona.

## Borrador, medir y comprobar

| Herramienta | Atajo | Notas |
|---|---|---|
| **Borrador** | `E` | Clic o arrastre sobre aristas. Borrar la arista disuelve las caras que dependían de ella. |
| **Cinta métrica** | `T` | Mide entre dos puntos y crea **guías** de construcción. |
| **Transportador** | `H` | Mide ángulos y crea guías angulares. |
| **Eliminar guías** | — | Edición ▸ Eliminar guías, cuando ya cumplieron su función. |

## Grupos y componentes

- **Agrupar** (`Ctrl+G`): la selección se vuelve un grupo — geometría aislada que no se "pega" al resto. **Doble clic** para entrar a editarlo; `Esc` o clic afuera para salir.
- **Desagrupar** (`Ctrl+Shift+G`) disuelve el grupo.
- **Componentes**: instancias que comparten definición — cambias una y cambian todas. Ideales para carpinterías, postes, árboles. Mover una instancia es O(1): el modelo no se duplica.
- Copiar y pegar (`Ctrl+C` / `Ctrl+V`) funciona entre documentos.

## Deshacer

`Ctrl+Z` / `Ctrl+Shift+Z` (o `Ctrl+Y`). **Toda** operación pasa por el historial — puedes retroceder siempre, incluso importaciones completas.
