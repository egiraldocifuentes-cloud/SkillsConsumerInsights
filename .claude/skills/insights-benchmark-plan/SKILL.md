---
name: insights-benchmark-plan
description: Define los jugadores y dimensiones de un benchmark competitivo (Fase 2 del flujo). A partir del encuadre cerrado, construye la lista justificada de competidores con Bancolombia como ancla obligatoria de comparación + 3–4 competidores por defecto (hasta 6 cuando la pregunta requiera lectura cuantitativa amplia como pricing, tasas o market share), y la matriz de dimensiones a comparar (núcleo: portafolio, propuesta de valor, CX, comunicación, pricing, performance pública; opcionales según pregunta). Aplica las reglas heredadas — Aval como conglomerado, CX obligatoria, internacional como inspiración no como competencia directa — y produce la matriz vacía lista para llenar en Fase 4. Usar después de `insights-benchmark-encuadre`, cuando se necesite traducir el alcance del benchmark en una matriz comparativa accionable.
---

# Skill: Plan de jugadores y dimensiones (Fase 2 del flujo)

## Filosofía aplicada
La selección de jugadores y dimensiones es el momento donde se decide **bisturí o escopeta**. Un benchmark con 15 jugadores y 12 dimensiones produce una tabla bonita pero poco accionable. Hay que justificar cada inclusión: por qué este jugador, por qué esta dimensión, qué decisión va a alimentar.

Leer `Flujo_Benchmark_Competitivo.md` y la Sección 4 del `Onboarding_Bancolombia_VP_Mercadeo.md` (mapa competitivo) antes de ejecutar la skill.

## Propósito
A partir del encuadre cerrado en Fase 1, construir:
- **Bancolombia siempre como ancla de comparación** + lista justificada de competidores (3–4 por defecto, hasta 6 cuando la pregunta lo justifique).
- Lista justificada de dimensiones a comparar (núcleo + opcionales según la pregunta).
- Matriz vacía (jugadores × dimensiones) lista para llenar en Fase 4.

## Regla de comparación base
**Todo benchmark de este flujo se construye con Bancolombia como referencia obligatoria.** El ejercicio nunca es "Nubank vs Lulo vs BBVA" en abstracto — es siempre "Bancolombia vs [X] vs [Y]". Bancolombia es la fila 0 de toda matriz. Sin esa ancla, el benchmark no alimenta una decisión del banco — describe el mercado en general, lo cual es otro tipo de trabajo.

## Cuándo invocar
- Cuando el encuadre se cerró con `insights-benchmark-encuadre` y el siguiente paso es definir el alcance comparativo.
- Cuando se está reusando un benchmark previo y hay que actualizar la lista de jugadores ante un cambio de mercado (ej. nuevo competidor, salida de un jugador como Scotiabank en 2025).

## Entradas que necesito
1. La **ficha de encuadre** cerrada (`BMK-YYYY-NN`) — incluyendo **ventana de observación**, **nivel de confidencialidad** y **tipo de ejercicio**.
2. Si el sponsor tiene jugadores específicos en mente, capturarlos.
3. Si el equipo o el sponsor ya tienen referencias internacionales en la cabeza, capturarlas.
4. Si el ejercicio es **cíclico** con edición previa, traer la matriz y los jugadores de la edición anterior para versionar la lista (qué se conserva, qué entra nuevo, qué sale).

## Estilo conversacional
Llegar con una **propuesta defendible**, no con preguntas en blanco. Proponer una lista preliminar de jugadores y dimensiones basada en el encuadre, justificarla, y discutirla con el usuario para ajustar.

## Pasos que debo ejecutar

### Paso 1 — Selección de jugadores

#### Bloque A — Competidores directos en Colombia (siempre que la geografía lo incluya)

Sugerir según el segmento del encuadre, referenciando el mapa del Onboarding (Sección 4):

| Segmento del banco | Competidores típicos a considerar |
|---|---|
| Banca Personas (Personal / Plus / Plus Alto) | Grupo Aval (consolidado), Davivienda / DAVIbank, BBVA, Itaú, Banco Caja Social, Nu Colombia, Lulo Bank, RappiPay |
| Preferencial / Banca Privada | BBVA Patrimonios, Itaú Privada, Davivienda Cuatro, Credicorp Capital |
| Pyme | Davivienda, BBVA, fintechs PYME (Finaktiva, Sempli) |
| Empresas / Corporativo | Grupo Aval (Bogotá, Occidente), Davivienda, BBVA, Itaú, Citi, Santander |
| Banca de Inversión | BTG Pactual, JPMorgan, Credicorp Capital |
| PSPs (cuando aplique Wompi) | PayU, ePayco, Mercado Pago, PlacetoPay |
| Marcas digitales (referencia para Nequi) | Daviplata, Nu, Lulo, dale!, RappiPay, Movii |

**Regla obligatoria:** si entran marcas de Grupo Aval (Bogotá, Occidente, Popular, AV Villas, dale!), agruparlas como **"Grupo Aval consolidado"** y leerlas a nivel holding — no marca a marca.

#### Bloque B — Referentes internacionales (cuando aplique)

Sugerir según la geografía del encuadre:

| Mercado | Referentes típicos |
|---|---|
| Brasil | Nubank, Itaú, Bradesco, C6 Bank, Banco Inter |
| México | Banorte, BBVA México, Klar, Hey Banco |
| España | BBVA, Santander, CaixaBank, Openbank, Bnext |
| EE. UU. / UK | Chime, Revolut, Monzo, Wise, SoFi |
| Otros faros globales | Tyme Bank (Sudáfrica), Kakao Bank (Corea), DBS (Singapur) |

**Regla obligatoria:** los referentes internacionales **NO son competencia directa** — entran como inspiración. Toda recomendación derivada de ellos se traducirá al contexto colombiano en Fase 5.

#### Bloque C — Anticipación competitiva (si el origen del encuadre es ese)

Si el encuadre marcó "Anticipación competitiva", agregar al menos 1–2 jugadores que sean **candidatos a entrar al mercado colombiano** — bancos / neobancos extranjeros con señales de aterrizaje (registro de marca, contrataciones locales, anuncios públicos, partnerships con jugadores locales). Documentar la señal específica que motiva la inclusión.

#### Validación de la lista
- **Bancolombia entra siempre como fila ancla.** No se cuenta en el tope de competidores.
- **Default: 3–4 competidores** además de Bancolombia. Es lo que permite profundidad real por celda en un ejercicio acotado de tiempo.
- **Hasta 6 competidores** cuando la pregunta lo justifique explícitamente — típicamente cuando se requiere **lectura cuantitativa amplia del mercado**: comparativos de pricing, tasas (ej. crédito hipotecario, libre inversión), market share, descargas, ratings transversales. Documentar la razón del aumento.
- **Más de 6 competidores se cuestiona.** Diluye profundidad y empuja al ejercicio a escopeta.
- Cada jugador entra con una justificación de **1 línea** ("se incluye porque…").
- Jugadores **descartados conscientemente** también se documentan ("no se incluye porque…") para trazabilidad.

### Paso 2 — Definición de dimensiones

#### Núcleo (siempre presentes salvo justificación de exclusión)
1. **Portafolio / propuesta de producto** — qué ofrece y a quién.
2. **Posicionamiento y propuesta de valor** — cómo se cuenta, qué promete.
3. **Experiencia de cliente (CX)** — onboarding, app, sucursal, atención post-venta. **Obligatoria.**
4. **Comunicación y narrativa pública** — campañas activas, redes sociales, voceros.
5. **Pricing / costos visibles al cliente** — cuotas de manejo, tasas, comisiones, beneficios.
6. **Performance pública cuando exista** — market share, descargas, ratings, NPS publicado, utilidades.

#### Opcionales según pregunta
- Sostenibilidad / ASG.
- Programas de lealtad y fidelización.
- Onboarding y conversión (si CX no lo cubre con suficiente profundidad).
- Innovación / portafolio digital nuevo.
- Cobertura territorial.
- Talento y marca empleadora.

#### Validación
- **Tope sugerido:** 5–7 dimensiones. Más diluye el bisturí.
- **CX siempre presente** salvo razón explícita registrada.
- Cada dimensión entra con un alcance acotado: qué SÍ mide, qué NO.

### Paso 3 — Construcción de la matriz vacía
Producir la matriz: filas = jugadores; columnas = dimensiones. Cada celda queda vacía y será llenada en Fase 4 con evidencia trazable.

### Paso 4 — Documentar el plan
Producir el entregable y archivarlo.

## Entregable

```
PLAN DE BENCHMARK #BMK-YYYY-NN
════════════════════════════════════════
Encuadre asociado: [BMK-YYYY-NN]
Fecha:
Ventana de observación heredada del encuadre: [...]
Nivel de confidencialidad: [Interno / Confidencial / Restringido]
Tipo de ejercicio: [One-off / Cíclico — cadencia / versión #]

JUGADORES SELECCIONADOS
─────────────────────────────────────────
| # | Jugador | Tipo | Justificación |
|---|---|---|---|
| 0 | **Bancolombia** | Ancla de comparación (siempre) | Referencia base del benchmark |
| 1 | [nombre] | Competidor directo / Referente internacional / Anticipación | [por qué entra — 1 línea] |
| 2 | ... | ... | ... |

Total competidores (sin contar Bancolombia): [N]
Default: 3–4 / Hasta 6 si la pregunta requiere lectura cuantitativa amplia
Si N > 4, justificación del aumento:

JUGADORES DESCARTADOS CONSCIENTEMENTE
─────────────────────────────────────────
| Jugador | Razón del descarte |
|---|---|

DIMENSIONES A COMPARAR
─────────────────────────────────────────
| # | Dimensión | Tipo | Alcance (qué SÍ / qué NO) |
|---|---|---|---|
| 1 | Portafolio / propuesta de producto | Núcleo | ... |
| 2 | Posicionamiento y propuesta de valor | Núcleo | ... |
| 3 | Experiencia de cliente (CX) | Núcleo (obligatoria) | ... |
| 4 | Comunicación y narrativa pública | Núcleo | ... |
| 5 | Pricing / costos visibles | Núcleo | ... |
| 6 | Performance pública | Núcleo | ... |
| 7 | [opcional] | Opcional | ... |

REGLAS HEREDADAS APLICADAS
─────────────────────────────────────────
[ ] Grupo Aval leído como conglomerado
[ ] Internacional marcado como inspiración (no competencia directa)
[ ] CX presente como dimensión obligatoria
[ ] Anonimización aplicada en todas las búsquedas externas

MATRIZ VACÍA
─────────────────────────────────────────
| Jugador \ Dimensión | D1 | D2 | D3 (CX) | D4 | D5 | D6 | ... |
|---|---|---|---|---|---|---|---|
| **Bancolombia** (ancla) | | | | | | | |
| [Competidor 1] | | | | | | | |
| [Competidor 2] | | | | | | | |
| ... | | | | | | | |

PRÓXIMO PASO
Próxima skill: insights-benchmark-fuentes
```

Guardar en: `Desktop/Gerencia Consumer Insights/Comparacion vs competidores/planes/<BMK-ID>-<titulo-corto>-plan.md`.

## Gate de salida
✅ Plan cerrado con: Bancolombia como ancla + 3–4 competidores justificados (hasta 6 si la pregunta lo justifica) + 5–7 dimensiones con alcance acotado + CX presente + Aval consolidado (si aplica) + matriz vacía construida + **ventana de observación / confidencialidad / tipo de ejercicio heredados del encuadre y visibles en el plan** + (si cíclico) versión y referencia a edición previa.

## Next step
- Continuar con `insights-benchmark-fuentes` (Fase 3) para mapear dónde buscar cada dimensión por jugador.

## Referencias
- `Flujo_Benchmark_Competitivo.md` — flujo completo y principios transversales.
- `Onboarding_Bancolombia_VP_Mercadeo.md` — Sección 4 (mapa competitivo por segmento).
- `Filosofia_Consumer_Insights.md` — criterios de bisturí vs escopeta.
- Memoria: `feedback_competidores_grupo_aval.md`, `feedback_incluir_experiencia_cliente.md`.
