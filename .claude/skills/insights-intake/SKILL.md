---
name: insights-intake
description: Recibe y triage una solicitud nueva de investigación de cualquier stakeholder de Bancolombia/Grupo Cibest. Estructura la necesidad, distingue si es trabajo reactivo (solicitud del stakeholder) o pista proactiva (oportunidad de tendencia), consulta si hay estudios previos que ya la resuelvan, y decide si se abre una investigación nueva o se cierra con data existente. Usar cuando llega un correo, reunión, ticket o mensaje de un stakeholder pidiendo información, research, un insight, una encuesta, un focus group, un estudio de marca, NPS, segmentación, pricing, concept test, etc.
---

# Skill: Intake de solicitud de investigación (Etapa 1 del flujo CI)

## Filosofía aplicada
Esta skill es la **primera línea de defensa** contra un problema común del área: que entre cualquier solicitud y se procese sin cuestionar si de verdad hay un insight que construir. Recordar siempre: **no somos mensajeros**. Si la solicitud no habilita una decisión estratégica, no se procesa — se devuelve o se cierra.

Leer `Filosofia_Consumer_Insights.md` y `Onboarding_Bancolombia_VP_Mercadeo.md` antes de ejecutar esta skill (al menos la primera vez de cada sesión).

## Propósito
Capturar de forma estructurada cualquier necesidad de información que llegue al equipo, aplicar triage y decidir el siguiente paso.

## Cuándo invocar
- Llega un correo/slack/reunión pidiendo "una encuesta", "un focus group", "entender a los clientes", "un estudio", "data de X", "validar una hipótesis".
- El sponsor dice "necesito saber…" o "quiero medir…" o "hay que investigar…".
- También: el equipo detecta una **señal externa** (tendencia, cambio de comportamiento, movimiento competitivo) y quiere decidir si abrir una investigación proactiva.

## Estilo conversacional
El equipo quiere que Claude **guíe el ejercicio con preguntas**, no que espere una descripción completa. Si el usuario pega un correo o describe la solicitud en forma libre, Claude debe:
1. Leer e identificar qué ya está dicho.
2. Hacer preguntas concretas agrupadas en 1–2 bloques (no una por una).
3. Cuestionar si es necesario (si falta la decisión de negocio, decirlo explícitamente).

## Entradas que debo pedir al usuario

### Si es reactivo (solicitud de stakeholder)
1. **Solicitante** (nombre y área/VP).
2. **Fecha requerida** y **criticidad** (alta / media / baja).
3. **Problema de negocio u oportunidad** que motiva la solicitud.
4. **Pregunta(s) clave** que el stakeholder quiere responder.
5. **Decisión** que habilitará la investigación (¿qué va a hacer el sponsor con el resultado?).
6. **Público objetivo** preliminar (segmento de banca de Bancolombia, región, producto, marca del grupo — ver segmentación oficial en onboarding).
7. **Presupuesto** tentativo.
8. **Estudios previos** que el sponsor conoce sobre el tema.

### Si es proactivo (tendencia detectada por el equipo)
En vez de "solicitante", capturar:
1. **Señal detectada** (qué se observó afuera).
2. **Fuente** (dónde se vio: social listening, prensa, estudio sindicado, conversación, comportamiento).
3. **Hipótesis inicial** de por qué podría impactar al banco.
4. **Segmento de banca o marca** potencialmente afectada.
5. **Nivel de urgencia** (¿es una tendencia emergente, estable o crisis?).

Si la entrada es proactiva → preferir invocar `insights-tendencias` como skill más específica.

## Pasos que debo ejecutar

1. **Leer el input** y extraer lo que ya viene descrito.
2. **Preguntar de forma concentrada** lo que falte — agrupado, no una a una.
3. **Aplicar triage** con este árbol de decisión:
   - ¿La pregunta ya tiene respuesta en estudios previos del repositorio? → **Cerrar con data existente** + recomendar qué estudio consultar.
   - ¿Se puede responder con data interna (CRM, transaccional, canales) sin campo? → **Redirigir a data analytics / BI**.
   - ¿La solicitud busca "traer el dato" sin decisión asociada? → **Devolver al sponsor** con la pregunta: *"¿qué decisión vas a tomar con esto?"* No somos mensajeros.
   - ¿Requiere investigación nueva y habilita una decisión? → **Abrir brief** (Etapa 2).
4. **Clasificar criticidad y esfuerzo** estimado en rejilla (Alto/Medio/Bajo impacto × Alto/Medio/Bajo esfuerzo).
5. **Validar los 5 criterios de calidad** de la filosofía (¿conecta puntos? ¿habilita acción? ¿hay mirada externa? etc.).
6. **Producir el entregable**.

## Entregable

```
SOLICITUD DE INVESTIGACIÓN #__
────────────────────────────────────────────────
Tipo: [ ] Reactivo (solicitud)  [ ] Proactivo (tendencia)
Solicitante / detector:
Área / VP:
Fecha de solicitud:
Fecha requerida:
Criticidad:

1. Problema de negocio u oportunidad
2. Pregunta(s) clave
3. Decisión que habilitará la investigación
4. Público objetivo preliminar (segmento: Personal 1-5MM / Plus 5-8MM / Plus Alto 8MM+ / Preferencial / Pyme / Empresas / Corporativo / Gobierno; marca: Bancolombia / Nequi / Sufi / Wompi / Wenia / Tuya / Renting)
5. Estudios previos conocidos
6. Presupuesto tentativo

TRIAGE
────────────────────────────────────────────────
Clasificación: [Abrir brief / Cerrar con data existente / Redirigir a BI / Devolver a sponsor]
Justificación:

FILTRO DE FILOSOFÍA (5 criterios)
[ ] Conecta puntos (no solo describe)
[ ] Llega a insight, no se queda en dolor
[ ] Habilita acción/decisión concreta
[ ] Requiere mirada externa (mercado/consumidor)
[ ] Es bisturí, no escopeta

Próximo paso:
Responsable sugerido:
```

Guardar en `Desktop/Gerencia Consumer Insights/solicitudes/SOL-YYYY-MM-DD-<titulo-corto>.md`.

## Gate de salida
✅ Solicitud estructurada + triage explícito + 5 criterios evaluados + responsable asignado.

## Next step
- Si triage = "Abrir brief" → sugerir `insights-brief`.
- Si es proactivo/tendencia → sugerir `insights-tendencias`.
- Si la necesidad se repite (brand tracking, NPS continuo) → sugerir `insights-brand-tracking`.

## Referencias
- `Anatomia_Insights.md` — framework formal (para evaluar si la solicitud permite construir insight o solo pide dato).
- `Filosofia_Consumer_Insights.md` — marco del equipo.
- `Flujo_Proceso_Consumer_Insights.md` (Etapa 1).
- `Onboarding_Bancolombia_VP_Mercadeo.md` — segmentos oficiales, marcas del grupo, stakeholders.
