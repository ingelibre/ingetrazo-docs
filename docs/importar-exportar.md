# Importar y exportar

## El formato nativo: `.igz`

Abierto y documentado. Sin texturas es JSON legible; con texturas se vuelve un contenedor autocontenido (las imágenes viajan **dentro**, sin rutas de tu máquina). Las composiciones de láminas, capas, escenas, BIM y georreferenciación se guardan ahí también. Guardado atómico: un corte de luz no corrompe el archivo.

## Importar SketchUp (`.skp`) — nativo

![Un `.skp` recién abierto: la geometría, los materiales y las capas originales de SketchUp llegan intactos.](images/import-sketchup.jpeg)


Archivo ▸ Importar ▸ SketchUp, o **doble clic** al archivo, o arrástralo a la ventana.

El importador es **propio y de código abierto** (proyecto [OpenSKP](https://github.com/iamahsanmehmood/openskp), al que IngeTrazo contribuye): lee el `.skp` directamente, **sin conversores ni SketchUp instalado**, en todas sus eras — desde los formatos antiguos (2013–2020) hasta los actuales.

Lo que llega:

- Geometría completa, **grupos y componentes** (las instancias siguen compartidas: mover una farola no arrastra el resto).
- **Materiales y texturas**, incluidos los colorizados, la translucidez, los materiales por lado y los billboards "siempre de cara".
- **Capas/etiquetas** con su visibilidad, **escenas** (cámara + capas por escena) y **cotas lineales**.
- Verificado con expedientes reales: bounding box exacto y 0.00 % de diferencia de área contra SketchUp.

!!! note "El conversor de respaldo"
    Para algún `.skp` exótico que el parser nativo aún no cubra, IngeTrazo ofrece automáticamente el conversor externo `skp2dae` (un clic para instalarlo). Es la excepción, no la regla.

## Otros formatos

| Formato | Importa | Exporta | Notas |
|---|:-:|:-:|---|
| **COLLADA (.dae)** | ✔ | ✔ | El export incluye la geolocalización — Blender lo abre con el sol de tu sitio para asoleamiento. |
| **OBJ** | ✔ | ✔ | Con materiales (MTL). |
| **STL** | — | ✔ | Binario, para impresión 3D. Sólidos herméticos garantizados. |
| **glTF / GLB** | — | ✔ | PBR + geolocalización; el formato de visores web y Blender moderno. |
| **IFC 4** | — | ✔ | El puente BIM. Ver [BIM y metrados](bim.md). |
| **DXF (R12)** | — | ✔ | La vista vectorial de una lámina, para IngeCAD/AutoCAD. Ver [láminas](laminas/exportar.md). |
| **Imagen** | — | ✔ | Captura de alta resolución del viewport. |
| **WebODM/ODM** | ✔ | — | El levantamiento de dron. Ver [Terreno](terreno/dron.md). |
| **CSV topográfico** | ✔ | — | Puntos P,N,E,Z de estación total. Ver [Terreno](terreno/rutas-perfil.md). |
| **KML / GeoJSON** | ✔ | — | Alineamientos y polígonos georreferenciados. |
