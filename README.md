# Pensamiento Crítico · skill de Claude

> **La IA que no te da la respuesta. Te da el criterio.**

La IA usada a demanda se asocia a peor pensamiento crítico (cognitive offloading). Usada con
estructura, lo amplifica. **Esta skill es la estructura**: un copiloto conversacional que
acompaña tu propio razonamiento, te caza suposiciones y solo interviene donde tu pensamiento
flojea. Lo técnico, eso sí, te lo resuelve al instante.

**Página explicada (interactiva):** https://luispitik.github.io/salgadoia-pensamiento-critico/

## El contrato, en 3 reglas

1. **Lo técnico, directo y al momento.** Errores, instalaciones, comandos: se resuelven sin rodeos.
2. **Lo de pensar, te lo entrena — no te lo hace.** Te hará preguntas, te cazará suposiciones
   y te pedirá que las ideas las digas tú.
3. **Tú tienes mandos.** Frases en lenguaje natural que la skill entiende y respeta (tabla abajo).

## Cómo funciona por dentro

No verás fases ni cuestionarios: hablas con normalidad y, por debajo, trabajan tres capas.

- **Clasificador silencioso** — cada mensaje se clasifica (técnico / conceptual / decisión /
  mal encaje / ambiguo) sin que lo notes. Lo técnico va directo; lo demás, al repertorio.
- **Dossier interno** — la skill anota tus afirmaciones literales (objetivos, criterios,
  datos pendientes) y lleva el contador de suposiciones cazadas.
- **7 movimientos** — en cada turno, **como máximo una corrección**, la de mayor valor.
  Dos correcciones seguidas son bolígrafo rojo, y el bolígrafo rojo mata la conversación.

| Movimiento | Qué hace |
|---|---|
| Afinado | Caza la palabra que no resiste un estándar de precisión — siempre con menú de opciones |
| Caza de supuestos | Lo que das por hecho, a la luz ("supuesto cazado, van 2") |
| Eco-espejo | Confronta dos frases tuyas que chocan, aunque las separen 14 turnos |
| Contrapeso | La perspectiva que falta — una, concreta y encarnada |
| Petición de esquema | El mapa lo dibujas tú con tus palabras; la skill solo audita con preguntas |
| Cierre con transferencia | 30 segundos que separan "hice la tarea" de "me la quedé" |
| Honestidad de encaje | "Para esto no soy yo" — y te deriva a la herramienta correcta |

Además: **regulación de estado** por inferencia conductual (fluido / comprimido / rojo con
"pagaré" para urgencias de adultos / fuera de juego ante malestar personal), **dos registros**
(adulto y adolescente — con menores la insistencia nunca desbloquea la respuesta) y **tres
niveles de autonomía** (N1 guiado → N2 auditado → N3 adversarial). El éxito de la skill se
mide en que la necesites cada vez menos: es un andamio que se retira.

## Instalación

### Claude Code (CLI / IDE)

```bash
# Global, para todos tus proyectos (Windows: %USERPROFILE%\.claude\skills\)
git clone https://github.com/Luispitik/salgadoia-pensamiento-critico.git ~/.claude/skills/salgadoia-pensamiento-critico

# O por proyecto
git clone https://github.com/Luispitik/salgadoia-pensamiento-critico.git .claude/skills/salgadoia-pensamiento-critico
```

Reinicia la sesión y verifica preguntando a Claude: *"¿qué skills tienes?"*

### Claude.ai y app de escritorio

1. Descarga `salgadoia-pensamiento-critico.skill` desde [Releases](https://github.com/Luispitik/salgadoia-pensamiento-critico/releases).
2. Ajustes → Capacidades → Skills → subir el archivo.
3. En la conversación: *"Activa pensamiento crítico"*.

## Uso

**Activación con configuración** (opcional, pensada para docentes):

> "Activa pensamiento crítico: registro adolescente, modo clase, nivel N1."

Sin configuración, los defaults son registro adulto, modo individual y nivel N2.

**Tus mandos** — frases que la skill entiende y respeta:

| Mando | Efecto |
|---|---|
| "guíame paso a paso" | Tarea troceada, un paso por turno |
| "dame una pista" | Pista, no solución — a cambio explicas qué cambia con ella |
| "estoy perdido" | Bloqueo legítimo: te ayuda a encontrar el primer paso |
| "simplifícamelo / estoy frito" | Modo comprimido: ella estructura, tú rellenas |
| "ERROR TÉCNICO: …" | Bypass garantizado: lo técnico se resuelve directo, siempre |
| "¿cómo voy?" | Tu marcador: suposiciones cazadas, pistas pedidas, qué te cuesta |
| "lo necesito ya" | (Adultos) Respuesta directa + un "pagaré": la próxima sesión explicas tú el porqué |
| "hazme de abogado del diablo" | Tú razonas, ella solo ataca tu conclusión |

## Para docentes

El paquete incluye despliegue en aula sin el creador delante:

- [`guia-docente.md`](guia-docente.md) — el script del contrato (tu diapositiva única),
  despliegue paso a paso, playbook de averías y el informe de proceso.
- [`guia-alumno.md`](guia-alumno.md) — 1 página imprimible con los derechos y mandos del alumno.

## La evidencia, en honesto

La tesis de la skill no es "la IA te atrofia": es que **el uso estructurado supera al uso
ingenuo**. El uso frecuente y no estructurado de IA se asocia (correlación, no causalidad
demostrada) a peor pensamiento crítico, mediado por cognitive offloading; las intervenciones
de IA con estructura muestran efectos grandes sobre el aprendizaje autorregulado. El motor
está construido sobre SRL (Zimmerman), Paul-Elder, ICAP (Chi & Wylie) y aprendizaje generativo
(Fiorella & Mayer), anclado al AILit Framework (Comisión Europea/OCDE) y al Art. 4 del EU AI Act.

Fuentes completas, calibradas y con contranarrativa incluida: [`references/fundamentos.md`](references/fundamentos.md).

## Privacidad y menores

- Con menores **no existe el "pagaré"**: insistir nunca desbloquea la respuesta directa.
- El informe docente habla **de proceso, nunca de contenidos personales**, y no hay
  persistencia de datos del menor por defecto.
- Ante señales de malestar personal, la skill declara su límite y deriva a una persona de
  confianza: es herramienta de aprendizaje, no de apoyo emocional.
- Como herramienta de alfabetización en IA se alinea con el Art. 4 del EU AI Act; si la
  despliegas en un centro, revisa además su política de protección de datos.

## Estructura del paquete

```
salgadoia-pensamiento-critico/
├── SKILL.md                        # El motor completo (lo que carga Claude)
├── guia-docente.md                 # Despliegue en aula + playbook de averías
├── guia-alumno.md                  # 1 página: derechos y mandos del alumno
├── references/
│   ├── banco-preguntas.md          # Paul-Elder operativo en español
│   └── fundamentos.md              # Evidencia calibrada con contranarrativa
└── docs/index.html                 # Página explicada (GitHub Pages)
```

## Licencia y autor

MIT — úsala, adáptala, despliégala en tu aula o tu empresa. Si la mejoras, los PR son bienvenidos.

**Luis Salgado** — psicólogo de formación y consultor de IA en activo (NorteIA · SalgadoIA).
Escribo sobre IA y mente humana en la newsletter **"IA con Cabeza"**.

---

*English summary: a Claude skill (Anthropic Skills format, Spanish-language) that turns Claude
into a critical-thinking tutor: it solves technical issues instantly but refuses to do your
conceptual thinking for you — it coaches it, one correction per turn, with evidence-based
scaffolding (SRL, Paul-Elder, ICAP, generative learning) that progressively removes itself.*
