# Instalación

IngeTrazo es gratuito y de código abierto (GPL-3.0). No pide cuenta, no tiene suscripciones y funciona sin internet.

## Windows

1. Descarga el instalador desde [ingetrazo.com](https://ingetrazo.com/#descargar) o desde los [releases de GitHub](https://github.com/ingelibre/ingetrazo/releases) (`ingetrazo-setup-vX.Y.Z.exe`).
2. Doble clic y sigue el asistente. El instalador asocia los archivos `.igz` y agrega IngeTrazo al menú "Abrir con" de `.skp` y `.dae`.
3. Si prefieres no instalar nada, descarga `ingetrazo-windows.zip` (versión portable): descomprime y ejecuta `ingetrazo.exe`.

!!! note "SmartScreen"
    La primera vez Windows puede mostrar el aviso de SmartScreen porque el instalador no está firmado comercialmente. Elige **Más información ▸ Ejecutar de todas formas**.

## Linux

Por ahora se instala desde el código fuente (el AppImage está en camino):

```bash
git clone https://github.com/ingelibre/ingetrazo.git
cd ingetrazo/app
python3 -m venv venv && venv/bin/pip install -r requirements.txt
venv/bin/python main.py
```

Para tener el ícono en el menú de aplicaciones y la asociación de archivos `.igz`/`.skp`/`.dae`:

```bash
scripts/install_desktop.sh
```

## macOS

IngeTrazo corre en macOS desde el código fuente con los mismos pasos que Linux. No hay todavía paquete `.dmg` oficial.

## Actualizar

- **Windows**: instala la versión nueva encima; conserva tus preferencias y asociaciones.
- **Linux**: `git pull` dentro de la carpeta del proyecto.

Tus modelos son archivos `.igz` normales en tu disco — actualizar el programa nunca los toca.
