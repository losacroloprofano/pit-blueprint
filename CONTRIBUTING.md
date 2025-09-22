# Contribuir al PIT Blueprint

## Flujo
1. Crear rama: `docs/nombre-corto`.
2. Editar Markdown en `docs/`. Mantener enlaces relativos.
3. Previsualizar local:
   ```bash
   source .venv/bin/activate
   mkdocs serve
   ```
4. Verificar build:
   ```bash
   mkdocs build --strict
   ```
5. Commit y push:
   ```bash
   git add .
   git commit -m "docs(scope): descripción"
   git push
   ```

## Estructura
- `docs/index.md` → Portada
- `docs/PIT-v3-MASTER.md` → Documento maestro
- `mkdocs.yml` → Configuración
- `.cursorrules` → Reglas para Cursor

## Calidad
- Build debe pasar `--strict`
- Enlaces internos verificados
- CI/CD automático en GitHub Actions

## Deploy
- Automático en Cloudflare Pages
- Para forzar redeploy: commit vacío
