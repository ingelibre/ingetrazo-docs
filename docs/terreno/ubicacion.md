# Ubicación del proyecto y mapa base

Todo el trabajo de terreno empieza fijando **dónde** está tu proyecto. Eso ancla el sistema de coordenadas y habilita el mapa satelital, el terreno 3D y los datos de campo.

## Fijar la ubicación

En la bandeja, panel **Terreno / Mapa base**:

1. **Buscar ubicación…** abre el localizador: busca el lugar por nombre, usa "Ubicarme", o navega el mapa.
2. Acomoda el mapa hasta que el **pin central esté exactamente sobre tu sitio** — haz zoom sin miedo.
3. Acepta y luego **Ir a ubicación**.

!!! warning "El pin ES el origen de tu modelo"
    El punto que eliges se convierte en el **origen (0,0,0)** del modelo. Dibuja alrededor del origen y tu modelo cae exactamente ahí sobre el satélite — sin tener que moverlo después. El propio mapa lo dice: el pin está rotulado *origen (0,0)*.

    Si el proyecto ya tenía ubicación y eliges otra, IngeTrazo **pregunta antes de mover el origen** (todo lo dibujado conserva sus coordenadas locales y se reubica sobre el mapa).

## Coordenadas: UTM o geográficas

Con el selector **Coordenadas** eliges cómo ver y escribir la posición — y el programa recuerda tu elección:

- **UTM WGS84**: Zona, hemisferio, **Este** y **Norte** — tal como lo reporta tu dron o tu estación total, con las convenciones estándar (falso este 500 km; falso norte 10 000 km en el hemisferio sur).
- **Geográficas**: latitud y longitud en grados decimales.

Ambos marcos están siempre sincronizados por debajo; cambiar de modo no pierde nada. Con el proyecto georreferenciado, la **barra de estado muestra la lectura UTM continua** del cursor.

## El mapa base

- **Fuentes**: satélite Esri, OpenStreetMap y las que agregues — cualquier servidor de teselas **XYZ** (tu propio ortofoto servido desde QGIS, por ejemplo) se guarda con nombre y queda para siempre en el menú.
- **Área de captura**: en el localizador puedes dibujar un rectángulo — un cuadrado para un sitio, una franja larga para una carretera.
- **Zoom** controla el detalle de las teselas; las capturas enormes reducen el detalle automáticamente para mantener el programa fluido.
- El mapa es **solo referencia visual**: nunca entra a tu geometría ni a tus metrados, y la captura se guarda con el documento (las teselas se descargan de nuevo al abrir).
