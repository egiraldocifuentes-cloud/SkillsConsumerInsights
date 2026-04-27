---
name: insights-analisis
description: Analiza la data levantada en campo (cuantitativa o cualitativa) y convierte hallazgos en insights accionables aplicando el framework Dolor→Tensión→Insight. Aplica técnicas estadísticas, codificación cualitativa, triangulación, conexión de puntos entre afuera (mercado/consumidor) y adentro (banco), y los criterios de calidad del equipo (relevante, novedoso, accionable, soportado; de escopeta a bisturí). Usar después de cerrar campo, o cuando el usuario diga "analizar data", "sacar insights", "qué dice la data", "procesar los resultados", "codificar las entrevistas".
---

# Skill: Análisis de data e insights (Etapa 5 del flujo CI)

## Filosofía aplicada
**Aquí es donde el equipo gana o pierde.** Si esta etapa queda en descripción ("el 62% dijo que…"), el equipo se vuelve mensajero. Si esta etapa construye insight con la anatomía formal del equipo, el equipo entrega bisturí.

**Framework formal obligatorio — INSIGHT = HECHO + MOTIVACIÓN + TENSIÓN**

Reglas no negociables:
- **No describir, interpretar.**
- **Todo insight debe tener sus tres componentes explícitos** (Hecho, Motivación, Tensión). Si falta uno, no es un insight — es un hallazgo o una opinión.
- **La motivación se nombra con marco teórico** (Maslow, Censydiam), no con intuición.
- **Conectar afuera (mercado/consumidor) con adentro (banco)** — la sinapsis que nadie más tiene.
- **Leer entre líneas** — el hallazgo obvio es hecho; el insight está una capa más profunda donde motivación y tensión se cruzan.

Leer obligatoriamente:
- `Anatomia_Insights.md` — teoría formal con definiciones, modelos y ejemplos.
- `Filosofia_Consumer_Insights.md` — principios del equipo.
- `Onboarding_Bancolombia_VP_Mercadeo.md` — segmentos, competencia, CX, stakeholders.

## Propósito
Convertir data en **insights accionables** que habiliten la decisión del sponsor.

## Cuándo invocar
- Campo cerrado, data lista.
- Hay que sacar insights, no solo tabulaciones.
- Preparar material para el informe.

## Estilo conversacional
Claude debe funcionar como **sparring del analista** usando la anatomía formal. Preguntas útiles:
- *"¿Qué te sorprendió? ¿qué no te cuadra?"*
- *"Este dato es el HECHO. ¿Cuál es la MOTIVACIÓN humana detrás? ¿Maslow? ¿Censydiam? ¿pertenencia, autocontrol, seguridad, logro?"*
- *"¿Qué TENSIÓN estorba esa motivación? ¿qué barrera está chocando?"*
- *"¿Con qué dinámica de afuera conecta esto? ¿qué está pasando en el consumidor colombiano que lo explica?"*
- *"Leamos entre líneas — ¿qué hay una capa más profunda?"*
- *"Si tuvieras que convencer al sponsor de una sola cosa, ¿cuál sería?"*
- *"¿Esto es insight o todavía es hallazgo? ¿tiene los tres componentes?"*

## Entradas
1. **Base limpia / transcripciones.**
2. **Brief original** (para volver al norte).
3. **Propuesta metodológica** (para cuotas y universo).
4. **Hipótesis iniciales** del sponsor.
5. **Contexto externo del periodo** (qué pasó en el banco, en la competencia, en CX, durante el campo) — crítico para conectar adentro con afuera.

## Pasos

### 5.1. Preparación

**Cuanti:** verificar limpieza, variables derivadas (segmentos, índices), ponderación, plan de tabulación por objetivo.
**Quali:** codificación abierta → axial → matrices por objetivo → patrones y contradicciones.

### 5.2. Análisis técnico

**Cuanti estándar:** frecuencias, cruces, significancia (chi², t-test, ANOVA), Top2Box / Bottom2Box, NPS (relacional vs transaccional), drivers (regresión, random forest).

**Cuanti avanzado:** segmentación (k-means, latent class), conjoint/MaxDiff, TURF, brand funnel, share of wallet.

**Quali:** análisis temático, verbatims representativos (no anecdóticos), mapas de empatía, customer journeys, arquetipos.

### 5.3. Integración híbrida
- Quali para explicar el **porqué** de lo cuanti.
- Cuanti para dimensionar la fuerza de lo quali.
- Triangulación entre perfiles y momentos.

### 5.4. De data a insight — el paso crítico (anatomía formal)

Para cada hallazgo importante, correr el ejercicio con la anatomía **Hecho + Motivación + Tensión**:

| Paso | Pregunta | Salida |
|---|---|---|
| 1. **Hecho** | ¿Qué dijo la data / el cliente? (verdad objetiva y verificable) | Dato, métrica, verbatim |
| 2. **Motivación** | ¿Qué necesidad humana profunda mueve esto? Nombrarla con Maslow o Censydiam. | Pertenencia / autocontrol / estima / seguridad / logro / poder / etc. |
| 3. **Tensión** | ¿Qué fricción, frustración o barrera estorba la motivación? ¿qué contradicción hay? | La fricción nombrada |
| 4. **Conexión afuera–adentro** | ¿Con qué dinámica del mercado/competencia/consumidor conecta? ¿qué del banco lo explica? | Puentes externos e internos |
| 5. **INSIGHT** | Síntesis narrativa que entrelaza hecho + motivación + tensión | Frase densa (ver ejemplos de `Anatomia_Insights.md`) |
| 6. **Implicación** | ¿Qué decisión concreta cambia? ¿qué botón hay que apretar? | Recomendación accionable |

**Criterio de validación:** si no puedo nombrar los tres componentes explícitamente, no tengo un insight; tengo un hallazgo. Volver a analizar.

### 5.5. Criterios de calidad del insight (4 filtros)

Antes de dejar un insight en el reporte:
- [ ] **Relevante** — conecta con el problema del brief.
- [ ] **Novedoso** — aporta algo que el sponsor no sabía.
- [ ] **Accionable** — permite decisión concreta.
- [ ] **Soportado** — tiene evidencia (dato + verbatim).

Si falla uno, bajar a "hallazgo secundario" o descartar.

### 5.6. Filtro de filosofía del equipo (5 criterios)

Transversal a todo el análisis:
- [ ] ¿Estoy conectando puntos o describiendo?
- [ ] ¿Llegué a insight o me quedé en dolor?
- [ ] ¿Hay acción posible?
- [ ] ¿Hay mirada de afuera explicando adentro?
- [ ] ¿Esto es bisturí (específico, dirigido) o escopeta (genérico)?

### 5.7. Construcción de narrativa

Estructura: `Contexto → pregunta del brief → hallazgos → insight → conexión afuera–adentro → implicación estratégica → decisión propuesta`.

Evitar ensalada de gráficas. Cada hallazgo lleva a un insight; cada insight a una decisión.

## Entregable

```
HALLAZGOS E INSIGHTS — <Nombre del estudio>
────────────────────────────────────────────────

CONTEXTO DEL ANÁLISIS
Qué pasó en el banco durante el periodo:
Qué pasó en la competencia:
Qué pasó en experiencia del cliente (canales, caídas, etc.):
Qué pasó en el consumidor / mercado:

────────────────────────────────────────────────

OBJETIVO 1: <del brief>
Hallazgos (descripción de lo que muestra la data):
  - …
  - …

ANATOMÍA DEL INSIGHT:
  Hecho:        [verdad objetiva — dato + verbatim]
  Motivación:   [necesidad humana profunda — nombrada con Maslow/Censydiam]
  Tensión:      [fricción/barrera que choca con la motivación]
  Conexión:     [con qué dinámica externa conecta; qué del banco lo explica]
  INSIGHT:      [síntesis narrativa que entrelaza los tres — una frase densa]
  Implicación:  [qué decisión cambia]

Filtro anatómico:
  [ ] Tiene Hecho explícito (dato verificable)
  [ ] Tiene Motivación explícita (con marco teórico)
  [ ] Tiene Tensión explícita (no asumida)
  [ ] Es una verdad profunda, no un hallazgo

Filtro de calidad del insight:
  [ ] Relevante [ ] Novedoso [ ] Accionable [ ] Soportado

OBJETIVO 2…
────────────────────────────────────────────────

HIPÓTESIS DEL SPONSOR — confirmación/refutación
  H1: [enunciado] → CONFIRMADA / REFUTADA / MATIZADA
      Evidencia:

────────────────────────────────────────────────

INSIGHTS TRANSVERSALES (no previstos)

────────────────────────────────────────────────

RECOMENDACIONES PRELIMINARES (bisturí)
  Decisión sugerida 1:
  Decisión sugerida 2:

FILTRO DE FILOSOFÍA DEL EQUIPO
[ ] Conecta puntos, no solo describe
[ ] Llega a insight, no se queda en dolor
[ ] Acciona decisión
[ ] Mirada externa explica interna
[ ] Bisturí, no escopeta
```

Guardar en `Desktop/Gerencia Consumer Insights/analisis/ANA-<codigo-estudio>.md`.

## Gate de salida
✅ Insights pasaron los 4 criterios de calidad + filtro de filosofía + revisión interna por otro analista o gerente.

## Buenas prácticas
- **Volver al brief siempre** — hallazgos jugosos fuera de brief van a anexos.
- **Cuidar la escala.** N=50 no da conclusiones estadísticas; en quali, 3 menciones no son patrón.
- **No confundir correlación con causalidad** en drivers.
- **Buscar las contradicciones** — son la materia prima de la tensión.

## Next step
Invocar `insights-informe`.

## Referencias
- `Anatomia_Insights.md` — framework formal Hecho + Motivación + Tensión + modelos (Maslow, Censydiam) + 3 ejemplos del equipo.
- `Filosofia_Consumer_Insights.md` — principios operativos + 5 filtros transversales.
- `Flujo_Proceso_Consumer_Insights.md` (Etapa 5).
- `Onboarding_Bancolombia_VP_Mercadeo.md` — contexto para conectar afuera con adentro.
