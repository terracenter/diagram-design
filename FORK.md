# Fork de seguridad de `diagram-design`

Fork mantenido por `terracenter`. Origen: https://github.com/cathrynlavery/diagram-design (MIT).
Punto de partida revisado: commit `b8f3617` (etiqueta `base-revisado-b8f3617`).

## Qué se quitó respecto al original

- `.github/` completo: workflows (incluido el bot de versiones con token), imágenes de PR y plantillas.
- `scripts/` de la raíz: herramientas de mantenimiento del autor; el skill no las usa al ejecutarse.
- Imágenes ráster de `docs/` (capturas y previsualizaciones). El README del original puede mostrar imágenes rotas.

No se tocó `skills/`, `commands/` ni `prompts/`. Se conservan `LICENSE` y los avisos de terceros.

## Política de uso

- Instalar siempre fijado a un commit de este fork; nunca seguir `main` del original.
- Exportar con `--system-fonts` y validar con `self_check.py --offline` (sin Google Fonts).
- Solo `.svg`; sin PNG ni Playwright.
- Actualizar desde el original solo tras revisar el diff completo.
- `/doctor` dentro de este repositorio reportará FAIL por los archivos de mantenimiento retirados; en un skill instalado funciona con normalidad.

## Pendiente

- Revisión línea por línea de los 6 scripts de `skills/diagram-design/scripts/`.
- Reemplazo de Python por el stack propio (PR aparte).
