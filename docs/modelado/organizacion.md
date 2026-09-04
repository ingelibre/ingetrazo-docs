# Capas, escenas y organización

## Capas

El panel **Capas** de la bandeja organiza la visibilidad del modelo:

- **+ Capa** crea una; el selector de cada entidad (o el panel Info de entidad) la asigna.
- El **ojo** muestra/oculta todo lo que vive en la capa — muebles, referencias, instalaciones.
- Al importar un `.skp`, las capas/etiquetas de SketchUp llegan con su visibilidad original.
- Eliminar una capa no borra su geometría: pasa a la capa por defecto.

!!! note "Capas = visibilidad, no aislamiento"
    Como en SketchUp, las capas controlan qué se ve; la geometría en capas distintas **sí se toca** si comparte espacio. Para aislar geometría usa **grupos**.

## Escenas

El panel **Escenas** guarda vistas con nombre:

- **+ Escena** captura la cámara actual **y** qué capas están ocultas.
- **Doble clic** en una escena la restaura.
- Las escenas se guardan en el `.igz`, llegan desde los `.skp` importados, y son las **fuentes de vista** del [compositor de láminas](../laminas/marcos.md): una escena "Planta" bien preparada es tu plano de planta.

## Info de entidad

El panel **Info** muestra y edita lo esencial de la selección: longitud de una arista, área de una cara, capa, material, y los metadatos BIM si los tiene.

## Estilo visual

- **Culling de caras**: los dorsos se pintan azul grisáceo para detectar caras volteadas de un vistazo.
- **Sombras y transparencias** se renderizan en el viewport tal como saldrán en el export de imagen.
- Vista ▸ **Exportar imagen** guarda una captura de alta resolución del viewport.

## Componentes: editas uno, cambian todos

Las copias de un componente (Ctrl+C / Ctrl+V, o Mover con Ctrl) comparten una misma definición. Como en SketchUp:

- **Doble clic en cualquier copia** la abre para editar. Dibuja, empuja, borra dentro; al salir (Esc o clic afuera), el cambio pasa a **todas** las copias. Toda la edición se deshace en un solo paso de Ctrl+Z.
- **Empujar/Tirar sobre una copia desde fuera** también edita la definición: las demás copias reciben el mismo empuje.
- **Para cambiar una sola copia**, antes de editarla usa clic derecho ▸ **Hacer único**: esa copia se desliga y las demás siguen compartiendo la definición.
- Mirar dentro de un componente y salir sin tocar nada no cambia nada.
