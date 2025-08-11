# PROYECTO_HTML_SITES

Repositorio para versionar:
- **/apps_script** → Google Apps Script (WebApp).
- **/sites_html** → HTML/CSS/JS para Google Sites.
- **/colab** → Notebooks y scripts Python para Google Colab.

## Objetivo
Tener control de versiones (historial, rollback y etiquetas) y un flujo simple de trabajo.

## Estructura
apps_script/   # Código de WebApps (clasp opcional)
sites_html/    # Archivos para Sites (src/dist si hace falta)
colab/         # .ipynb y /src con funciones reutilizables
CHANGELOG.md   # Historial de cambios
.gitignore     # Archivos que no se suben

## Flujo básico (Git)
# traer cambios antes de empezar
git pull origin main
# añadir cambios
git add .
# guardar con mensaje claro
git commit -m "feat: detalle del cambio"
# subir a GitHub
git push origin main

## Versionado (SemVer)
- MAJOR.MINOR.PATCH
  - MAJOR: cambios incompatibles
  - MINOR: nuevas funciones compatibles
  - PATCH: correcciones
- Mantener CHANGELOG.md.
- (Opcional) etiquetas:
  git tag v1.0.0
  git push origin v1.0.0

## Checklist
- Código probado
- CHANGELOG.md actualizado
- Commit con mensaje claro
- git push origin main

## Tips
- Git no sube carpetas vacías → usamos .gitkeep
- En Sites, pegar archivos de /sites_html
- En Colab, mover lógica a /colab/src/*.py
