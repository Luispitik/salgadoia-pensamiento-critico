# salgadoia-pensamiento-critico

Skill de Claude (formato Anthropic Skills, en español): tutor conversacional de pensamiento
crítico. Repo público — la fuente de verdad de la skill publicada.

## Estructura

- `SKILL.md` — el motor (frontmatter + reglas). Es lo único que carga el modelo siempre.
- `references/` — material bajo demanda: banco de preguntas Paul-Elder y fundamentos científicos.
- `guia-docente.md` / `guia-alumno.md` — documentación para humanos, no para el modelo.
- `docs/index.html` — página explicada, servida como GitHub Pages.

## Convenciones

- Todo en español; el diseño de la skill exige cirugía al editar: respeta el principio
  "una corrección por turno" también en el texto (cambios mínimos, estilo del documento).
- Todo claim científico va en `references/fundamentos.md` con fuente primaria y calibración
  Alto / Medio / Contranarrativa. Sin fuente primaria no entra.
- Versionado semántico en `CHANGELOG.md`. Cada versión se publica como GitHub Release con el
  `.skill` adjunto (ZIP de la carpeta `salgadoia-pensamiento-critico/` con SKILL.md, guías y
  references/, renombrado a `.skill`).
- Las guías y el SKILL.md deben mantenerse sincronizados: cada mando o promesa de las guías
  tiene que existir como regla en el motor.
