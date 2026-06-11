# Guía del docente · Skill de Pensamiento Crítico

**Para quién:** docente que despliega la skill en aula (instituto, universidad o formación de
adultos) sin el creador delante. **Tiempo de preparación realista: 2-3 horas dentro de tus
48 h.** No necesitas saber programar; necesitas entender el contrato y saber qué hacer cuando
un alumno la rompa.

## 1. Qué es (y qué no es) — 1 minuto

Es un tutor conversacional que acompaña al alumno mientras trabaja: le resuelve al instante lo
técnico (errores, instalaciones) y le entrena lo conceptual señalándole objetivos difusos,
suposiciones sin comprobar y contradicciones — **sin darle las respuestas hechas**. No es un
ChatGPT capado: es una IA con un contrato distinto, y tu trabajo nº 1 es presentar ese
contrato ANTES de que la usen. Si lo descubren rompiéndose su expectativa, la percibirán
como una IA defectuosa y la guerra está perdida.

## 2. El script del contrato (tu diapositiva única — léelo casi literal)

> "Vais a trabajar con una IA que funciona distinto a las que conocéis. Tres reglas:
> **Uno** — lo técnico os lo resuelve al momento: errores, instalaciones, comandos. Pedídselo
> sin miedo. **Dos** — lo de pensar NO os lo hace: os lo entrena. Os hará preguntas, os cazará
> suposiciones, y el trabajo que salga será VUESTRO — que es exactamente lo que hace que no
> suene al mismo trabajo que el de los otros 30. **Tres** — tenéis derechos: podéis decirle
> 'guíame paso a paso', 'dame una pista' o 'estoy perdido', y se adapta. Lo que no funciona
> es insistir para que os lo haga: eso lo tiene prohibido conmigo."

Con adultos, sustituye el argumento de la nota por el del criterio: "saldréis con una decisión
que podéis defender, no con una respuesta que no sabríais justificar".

## 3. Despliegue — paso a paso

1. Instala la skill en el entorno de la clase (carpeta `salgadoia-pensamiento-critico/` con
   su `SKILL.md` en el directorio de skills; reinicia la sesión; verifica preguntando a la IA
   "¿qué skills tienes?").
2. Decide la configuración de la sesión y dícsela a la IA en el primer mensaje:
   - **Registro:** `adolescente` o `adulto`.
   - **Modo:** `clase` (consultas de 3-5 min, recomendado en aula) o `individual`.
   - **Nivel:** N1 guiado (primera vez, recomendado) / N2 auditado / N3 adversarial.
   Ejemplo: *"Activa pensamiento crítico: registro adolescente, modo clase, nivel N1."*
3. Proyecta la diapositiva del contrato y léela.
4. Reparte la guía del alumno (1 página) o déjala abierta en sus pantallas.
5. Lanza la tarea. Tú circulas: la IA absorbe las dudas técnicas y de comprensión; tú te
   quedas con lo importante — los atascados de verdad y la dinámica de grupo.

## 4. Playbook de averías (qué hacer cuando se rompe)

| Síntoma | Qué pasa | Qué haces |
|---|---|---|
| "La IA no me contesta, solo pregunta" | El alumno esperaba respuestas (contrato no calado) | Repite la regla 2 del contrato en 10 segundos y enséñale a pedir "dame una pista". |
| "Le he pedido el trabajo y no me lo hace" | Guardrail funcionando | Es la skill haciendo su trabajo. Redirige: "pídele que te lo trocee en pasos". |
| Alumno bloqueado con error técnico y la IA no lo resuelve | Mensaje ambiguo: la IA no detectó que era técnico | Que lo reformule: "dile literalmente: ME DA ERROR, y pega el error". |
| La IA suelta preguntas filosóficas a un error de instalación | Fallo de clasificación (raro) | Mismo remedio: mensaje empezando por "ERROR TÉCNICO:". Apúntalo para reportarlo. |
| Varios alumnos con el mismo atasco | Problema de material, no de skill | Para la clase 2 min y resuélvelo en pizarra; la guía del alumno debe cubrirlo la próxima vez. |
| Un alumno insiste e insiste para sacar la respuesta | Intento de bypass | La skill no cede (en menores no existe el "pagaré"). Si persiste, la skill lo deriva a ti: es tu conversación, no la suya. |
| Un alumno cuenta a la IA un problema personal | Límite de la skill | La skill corta con calidez y sugiere hablar con una persona de confianza. Esa persona eres tú: atiéndelo. |

## 5. El informe de proceso (tu trazabilidad)

Al cierre de una sesión guiada puedes pedir a la IA el informe de proceso del grupo o del
alumno: qué suposiciones cazó solo, dónde necesitó pistas, qué le costó más (precisar, asumir
perspectivas, conectar). **Habla de proceso, nunca de contenidos personales.** Úsalo para
decidir quién sube de nivel (N1→N2→N3): el objetivo del sistema es que dejen de necesitar
el andamio, no que dependan de él.

## 6. Errores de docente que matan la skill

- Presentarla como "un ChatGPT para clase". Crea la expectativa exactamente contraria.
- Saltarse el contrato "porque no hay tiempo". Son 40 segundos; sin ellos pierdes la sesión.
- Usarla para vigilar contenidos de los alumnos. El informe es de proceso; pedirle más rompe
  la confianza y, con menores, la privacidad.
- Dejar a toda la clase en N1 para siempre. Si en 3-4 sesiones nadie sube a N2, el andamio se
  ha vuelto muleta: fuerza la subida.

## 7. Preguntas frecuentes

**¿Necesito la guía del alumno si la skill ya les ayuda?** Sí: la guía cubre el procedimiento
paso a paso (instalar, abrir, ejecutar) en autoservicio visual; la skill cubre comprensión y
tarea. Son piezas distintas: pantalla estática para el "no me arranca", conversación para el
"no lo entiendo".

**¿Puedo adaptar las preguntas o el tono?** Sí: el banco de preguntas
(`references/banco-preguntas.md`) es editable y la skill acepta instrucciones de configuración
en el primer mensaje.

**¿Y si me preguntan por la evidencia científica?** Está resumida y citada en
`references/fundamentos.md`. Versión de 10 segundos: "la IA sin estructura erosiona el
pensamiento crítico; con estructura, lo amplifica — esto es la estructura".
