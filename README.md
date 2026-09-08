# Manual de IngeTrazo (docs)

Sitio de documentación de usuario, hecho con [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).
Hermano de `ingepresupuestos-docs` (docs.ingepresupuestos.com): mismo stack y convenciones.

## Desarrollo local

```bash
python3 -m venv venv
venv/bin/pip install -r requirements.txt
venv/bin/mkdocs serve        # http://127.0.0.1:8000
```

Editar el contenido en `docs/` (Markdown). La navegación se define en `mkdocs.yml`.

## Publicar (Cloudflare Pages, subida directa)

El proyecto `ingetrazo-docs` de Cloudflare Pages **NO está conectado a
GitHub**: un `git push` no construye nada (comprobado el 2026-09-07). Se
construye aquí y se sube la carpeta `site/` con wrangler:

```bash
venv/bin/mkdocs build
npx wrangler pages deploy site --project-name ingetrazo-docs --branch main
git push   # el repo es solo el historial del fuente
```

- **Output directory:** `site` (ignorada por git)
- **URL:** https://ingetrazo-docs.pages.dev · **Dominio previsto:** docs.ingetrazo.com
