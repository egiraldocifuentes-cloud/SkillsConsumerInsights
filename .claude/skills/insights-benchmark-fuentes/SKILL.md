---
name: insights-benchmark-fuentes
description: Mapea y prioriza las fuentes de información para un benchmark competitivo (Fase 3 del flujo). A partir del plan cerrado en Fase 2 (Bancolombia + competidores + dimensiones), decide DÓNDE se va a buscar cada celda de la matriz combinando un catálogo base (sitios web oficiales, apps y tiendas, redes sociales corporativas, comunidades y foros en línea, sitios de reseñas, reportes regulatorios SFC y Asobancaria, prensa especializada, reportes de consultoras y mystery shopping ligero) con las fuentes que aporte el usuario (enlaces, documentos de referencia, artículos, reportes internos, estudios previos). Aplica reglas de anonimización (queries en lenguaje neutro, sin mencionar Bancolombia) y triangulación (mínimo 2 tipos de fuente por dimensión). Produce el plan de fuentes con queries propuestas listo para ejecutar en Fase 4. Usar después de `insights-benchmark-plan`, antes de empezar el desk research.
---

# Skill: Mapeo de fuentes de benchmark (Fase 3 del flujo)

## Filosofía aplicada
Decidir **dónde se busca antes de empezar a buscar** evita el desk research errático y garantiza profundidad por dimensión. Una buena celda de la matriz es la que tiene fuente trazable y triangulada — no la que tiene "lo que apareció primero en Google".

Leer `Flujo_Benchmark_Competitivo.md` (Fase 3) antes de ejecutar la skill.

## Propósito
A partir del plan cerrado en Fase 2, producir el **plan de fuentes**: tabla cruzando dimensión × jugador × fuentes priorizadas, con queries en lenguaje neutro listas para ejecutar.

## Cuándo invocar
- Inmediatamente después de cerrar `insights-benchmark-plan`.
- Cuando se reusa un benchmark previo y hay que actualizar las fuentes (links rotos, fuentes nuevas, dimensiones nuevas).

## Entradas que necesito
1. El **plan de benchmark cerrado** (`BMK-YYYY-NN-plan`).
2. La matriz vacía con jugadores y dimensiones definidas.
3. **Fuentes aportadas por el usuario** — cuando el usuario tenga material de partida, capturarlo y tratarlo como fuente prioritaria del plan. Esto incluye:
   - Enlaces (URLs de artículos, reportes, posts, papers, blogs especializados, hilos en redes, videos).
   - Documentos de referencia (PDFs, Word, presentaciones, dossiers de la gerencia).
   - Estudios previos del repositorio interno o de aliados.
   - Cuentas o comunidades específicas que el equipo ya monitorea.
   - Personas / voceros / analistas que el equipo sigue como referencia.
   La skill **acepta e integra** estas fuentes; no las descarta para usar solo el catálogo base.

## Estilo conversacional
Llegar con un mapeo defendible por defecto y discutirlo. Sugerir fuentes específicas por dimensión, no preguntar "¿dónde buscamos?". El equipo debería poder decir "agreguemos X" o "saquemos Y", no construir desde cero.

**Preguntar siempre, antes de proponer:** *"¿Tienes algún enlace, documento o referencia que quieras que incorporemos como fuente?"* Si el usuario pega una URL, comparte un PDF o menciona un reporte específico, esa fuente entra al plan con prioridad y se etiqueta como "aportada por el usuario".

## Catálogo de fuentes (referencia para mapear)

| Tipo de fuente | Qué se obtiene | Para qué dimensiones sirve mejor | Ejemplos |
|---|---|---|---|
| **Sitios web oficiales y portales de inversionistas** | Portafolio declarado, propuesta de valor, segmentos, indicadores corporativos | Portafolio, posicionamiento, performance | Página corporativa de cada entidad, sección de relación con inversionistas, reportes anuales / 20-F |
| **Apps móviles y tiendas de aplicaciones** | UX, funcionalidades, ratings, reviews, frecuencia de actualización | CX, innovación, onboarding | App Store, Google Play, capturas y prueba directa |
| **Redes sociales corporativas** | Narrativa, frecuencia, tono, engagement, públicos a los que apela | Comunicación, posicionamiento | LinkedIn, X, Instagram, TikTok, YouTube, Facebook |
| **Comunidades, foros y grupos en línea** | Voz no filtrada del cliente, fricciones reales, comparaciones espontáneas | CX, pricing percibido, posicionamiento | Reddit (r/Colombia, r/personalfinance, r/finanzas), Quora, grupos públicos de Facebook, comunidades de Telegram / Discord |
| **Sitios de reseñas y comparación** | Comparativos de pricing, reviews, rankings sectoriales | Pricing, CX | Rankia, Trustpilot, comparadores de tasas, blogs de finanzas personales |
| **Reportes oficiales y regulatorios** | Cifras duras: market share, cartera, morosidad, indicadores de inclusión | Performance, market share | Superintendencia Financiera (SFC), Asobancaria, Banco de la República, Fogafín, Colombia Fintech |
| **Prensa especializada y analistas** | Movimientos estratégicos, M&A, lanzamientos, controversias, señales de aterrizaje de nuevos competidores | Posicionamiento, anticipación, performance | Portafolio, La República, Valora Analitik, Bloomberg Línea, El Colombiano, Reuters, Financial Times |
| **Reportes de industria y consultoras** | Tendencias regionales y globales, benchmarks transversales | Inspiración internacional, posicionamiento | McKinsey, BCG, Bain, Deloitte, Capgemini (World Retail Banking Report), Finnovista, EY |
| **Mystery shopping ligero (opcional)** | Validación de fricciones reales en onboarding, atención o conversión | CX, onboarding, pricing efectivo | Apertura de cuenta de prueba, simulación de chat, llamada al call center |

## Pasos que debo ejecutar

### Paso 1 — Recoger fuentes aportadas por el usuario
Antes de mapear desde el catálogo, preguntar explícitamente al usuario si tiene fuentes propias (enlaces, documentos, reportes, cuentas, voceros). Si las tiene:
- Capturarlas con su contexto: ¿qué dimensión alimenta?, ¿qué jugador?, ¿por qué la trajo?
- Si es un PDF o documento local, leerlo (con `Read`) y resumir el aporte que hace al benchmark.
- Si es una URL, capturarla con la fecha y una nota corta del contenido relevante.
- **Estas fuentes entran como prioritarias y no cuentan dentro del catálogo base** — son adicionales, no sustitutas (salvo que el usuario indique lo contrario).

### Paso 2 — Asignación de fuentes por dimensión (catálogo + aportadas)
Para cada dimensión definida en Fase 2, asignar **al menos dos tipos de fuente** (regla de triangulación). Combinar las fuentes aportadas por el usuario (Paso 1) con sugerencias del catálogo.

Ejemplo de asignación:
- **CX** → Apps + Comunidades online + Sitios de reseñas (mínimo).
- **Pricing** → Sitios oficiales + Sitios de reseñas + Reportes regulatorios.
- **Comunicación** → Redes sociales corporativas + Prensa especializada.
- **Performance pública** → Reportes regulatorios (SFC, Asobancaria) + Prensa especializada.
- **Posicionamiento** → Sitios oficiales + Reportes de consultoras + Redes sociales.

### Paso 3 — Asignación de fuentes por jugador (matiz por jugador)
Algunas fuentes solo aplican a algunos jugadores:
- **Reportes regulatorios SFC / Asobancaria** → solo entidades reguladas en Colombia.
- **Reportes 20-F / SEC** → solo entidades listadas en bolsa de EE. UU. (Cibest, Davivienda, Itaú, etc.).
- **Prensa local internacional** → según mercado del referente (Brasil → Folha, Valor; México → El Economista; etc.).

Para cada jugador, marcar qué fuentes del catálogo aplican.

### Paso 4 — Redacción de queries con anonimización

**Regla obligatoria:** toda búsqueda en fuentes externas y todo prompt a herramientas de IA externas se redacta en **lenguaje neutro**. **No mencionar Bancolombia ni Grupo Cibest** como origen del análisis. (Memoria: `feedback_anonimizacion_desk_research.md`.)

**Ejemplos de redacción:**

| ❌ NO usar | ✅ Usar en su lugar |
|---|---|
| "Cuáles son las ventajas de Nubank vs Bancolombia" | "Comparativo de neobancos en Colombia: posicionamiento y propuesta de valor" |
| "Por qué Bancolombia pierde clientes jóvenes frente a Nu" | "Tendencias de adopción de neobancos en Colombia entre Gen Z y Millennials" |
| "Reseñas de la app de Bancolombia vs competencia" | "Reseñas y ratings de apps bancarias en Colombia 2025" |

Para cada celda de alta prioridad, redactar 1–2 queries listas para ejecutar.

### Paso 5 — Idioma de fuentes internacionales

Para referentes internacionales, las fuentes pueden estar en idioma original (portugués para Brasil, inglés para EE. UU./UK, coreano para Corea, etc.). Reglas:

- **Capturar el link y la captura en idioma original** — la URL no se traduce.
- **Citas textuales se conservan en idioma original entre comillas**, con una **traducción libre debajo** entre paréntesis.
- **Nombres de productos, marcas y términos regulatorios no se traducen** (ej. "Pix", "PIX", "Cajitas de Nu", "SEDPE").
- **Para reportes largos:** registrar la fuente, leer en original (con apoyo de traducción si es necesario para entender), y citar fragmentos clave en idioma original con traducción libre.
- **No usar herramientas de traducción para sustituir cita textual** — pueden alterar matices regulatorios o de tono.
- En el log de búsqueda, marcar el idioma de cada fuente útil.

### Paso 6 — Priorización temporal y de profundidad
- **Respetar la ventana de observación definida en el encuadre.** Toda fuente cuya fecha caiga fuera de la ventana se descarta o se marca como "contexto histórico fuera de ventana".
- Si la ventana es muy estrecha (ej. últimos 3 meses) y no hay material suficiente, **devolver al sponsor**: ¿se amplía la ventana o se acepta menos profundidad?
- Para **anticipación competitiva**, la ventana hacia atrás suele ser corta; pero el horizonte proyectado puede requerir referencias históricas externas (ej. cómo Nubank entró a México hace 3 años) — esas referencias entran como contexto explícito, no como evidencia comparativa.
- Marcar celdas de **alta profundidad** (las que alimentan los insights core) vs **baja profundidad** (contexto suficiente).

### Paso 7 — Documentar el plan de fuentes
Producir el entregable.

## Entregable

```
PLAN DE FUENTES #BMK-YYYY-NN
════════════════════════════════════════
Plan asociado: [BMK-YYYY-NN-plan]
Fecha:
Ventana de observación heredada: [...]
Nivel de confidencialidad: [Interno / Confidencial / Restringido]

FUENTES APORTADAS POR EL USUARIO
─────────────────────────────────────────
| # | Fuente (link / doc / cuenta / vocero) | Tipo | Dimensión / jugador que alimenta | Nota del contenido relevante |
|---|---|---|---|---|
| 1 | [URL o nombre del documento] | Enlace / PDF / Cuenta / Vocero / Estudio previo | [dimensión] / [jugador] | [resumen de 1 línea] |
| ... | ... | ... | ... | ... |

(Si no hay fuentes aportadas, dejar la tabla vacía y marcarlo explícitamente.)

ASIGNACIÓN POR DIMENSIÓN (catálogo + aportadas)
─────────────────────────────────────────
| Dimensión | Tipos de fuente asignadas (mín. 2) | Fuentes aportadas que aplican | Profundidad esperada |
|---|---|---|---|
| Portafolio | Sitio oficial + Reportes anuales | [#] | Alta |
| Posicionamiento | Sitio oficial + Redes sociales + Prensa | [#] | Alta |
| CX | Apps + Comunidades + Reseñas | [#] | Alta |
| Comunicación | Redes sociales + Prensa | [#] | Media |
| Pricing | Sitios oficiales + Reseñas + Reportes regulatorios | [#] | Alta |
| Performance | Reportes regulatorios + Prensa | [#] | Alta |
| ... | ... | ... | ... |

ASIGNACIÓN POR JUGADOR (matiz)
─────────────────────────────────────────
| Jugador | Fuentes que aplican | Fuentes que NO aplican |
|---|---|---|
| Bancolombia | Todas | — |
| [Competidor Colombia] | Todas | — |
| [Referente internacional] | Sitio + Redes + Prensa local + Consultoras | SFC / Asobancaria (no regulado en Colombia) |
| ... | ... | ... |

QUERIES PRIORITARIAS (anonimizadas)
─────────────────────────────────────────
| Dimensión | Jugador / contexto | Query propuesta |
|---|---|---|
| CX | Apps bancarias Colombia | "reseñas app bancaria Colombia 2025 fricciones onboarding" |
| Pricing | Crédito hipotecario | "tasas crédito hipotecario bancos Colombia 2025 comparativo" |
| Comunicación | Neobancos LATAM | "campañas redes sociales neobancos LATAM 2025 narrativa" |
| ... | ... | ... |

REGLAS APLICADAS
─────────────────────────────────────────
[ ] Fuentes aportadas por el usuario capturadas e integradas (o tabla vacía marcada explícitamente)
[ ] Mínimo 2 tipos de fuente por dimensión (triangulación)
[ ] Queries redactadas en lenguaje neutro (anonimización)
[ ] Ventana de observación del encuadre respetada en la priorización temporal
[ ] Idioma de fuentes internacionales documentado (capturas en idioma original)
[ ] Profundidad alta marcada en dimensiones core

PRÓXIMO PASO
Próxima skill: insights-benchmark-desk (y/o insights-benchmark-social para redes y comunidades)
```

Guardar en: `Desktop/Gerencia Consumer Insights/Comparacion vs competidores/fuentes/<BMK-ID>-<titulo-corto>-fuentes.md`.

## Gate de salida
✅ Plan de fuentes cerrado con: fuentes aportadas por el usuario integradas (o ausencia explícita) + cada dimensión con ≥2 tipos de fuente + queries anonimizadas listas para ejecutar + matiz por jugador documentado + profundidad esperada marcada.

## Next step
- Continuar con `insights-benchmark-desk` (Fase 4a) para ejecutar el desk research general.
- En paralelo (o secuencial según el caso), invocar `insights-benchmark-social` (Fase 4b) para el monitoreo de redes y comunidades online.

## Referencias
- `Flujo_Benchmark_Competitivo.md` — Fase 3, catálogo de fuentes y reglas de mapeo.
- Memoria: `feedback_anonimizacion_desk_research.md` — regla obligatoria de lenguaje neutro en queries externas.
- `Onboarding_Bancolombia_VP_Mercadeo.md` — fuentes específicas referenciadas en el banco (SFC, Asobancaria, etc.).
