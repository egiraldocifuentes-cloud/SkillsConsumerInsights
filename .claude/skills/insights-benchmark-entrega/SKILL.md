---
name: insights-benchmark-entrega
description: Construye el entregable final del benchmark competitivo (Fase 6 del flujo) en forma de reporte HTML interactivo con marca Bancolombia, usando como base la plantilla `reporte_competitivo_bancolombia.html` ubicada en la carpeta madre `Gerencia Consumer Insights/`. Toma todos los productos del análisis (encuadre, plan, fuentes, levantamiento desk + social, retos, insights con anatomía formal, recomendaciones bisturí, anticipación competitiva, hipótesis abiertas) y los traduce a las secciones del reporte: resumen ejecutivo, encuadre, metodología, hallazgos por dimensión, análisis por jugador, anticipación, retos, insights, recomendaciones y anexo de evidencia. Valida reglas de marca (amarillo siempre presente, sin degradados, Negro CIB sobre blanco, Inter como tipografía estándar de la plantilla) y archiva con metadatos para reuso. Identifica hipótesis abiertas que valdría derivar al flujo reactivo (`insights-intake`). Usar como cierre del flujo de Benchmark Competitivo, después de `insights-benchmark-analisis`.
---

# Skill: Entrega y archivo del benchmark (Fase 6 del flujo)

## Filosofía aplicada
La entrega no es solo presentar — es **dejar el conocimiento utilizable**. Un reporte HTML bien estructurado:
- Permite al sponsor leer en su tiempo, sin reunión obligatoria.
- Sostiene los insights con evidencia clickeable.
- Queda en el repositorio listo para reuso futuro.
- Refleja la marca Bancolombia con disciplina visual.

No se entrega lo que no pasó por los 5 filtros del equipo (validados en Fase 5).

Leer `Flujo_Benchmark_Competitivo.md` (Fase 6) antes de ejecutar.

## Propósito
Construir el reporte HTML interactivo con marca Bancolombia y archivarlo con metadatos para que el conocimiento quede reusable. Cerrar el ciclo identificando hipótesis abiertas que justifiquen abrir investigación primaria.

## Cuándo invocar
- Cuando `insights-benchmark-analisis` está cerrada con sus 5 filtros aplicados.
- Cuando se quiere actualizar un reporte previo con datos nuevos.

## Entradas que necesito
1. **Análisis cerrado** (`BMK-YYYY-NN-analisis`) — incluye lecturas vertical/horizontal, retos, insights con anatomía, recomendaciones, traducción internacional, hipótesis abiertas.
2. **Encuadre** (`BMK-YYYY-NN`) — para resumen ejecutivo y sección de alcance.
3. **Plan** (`BMK-YYYY-NN-plan`) — jugadores, dimensiones, matriz.
4. **Plan de fuentes** (`BMK-YYYY-NN-fuentes`) — para sección de metodología.
5. **Levantamientos** (`BMK-YYYY-NN-levantamiento` y `BMK-YYYY-NN-social`) — matriz diligenciada, capturas, verbatims.
6. **Plantilla HTML base:** `Desktop/Gerencia Consumer Insights/reporte_competitivo_bancolombia.html`.

## Estilo conversacional
Llegar con un esqueleto del HTML ya armado a partir del análisis. Discutir con el usuario si hay secciones a destacar, KPIs específicos a poner en el header, o callouts adicionales. No empezar desde cero ni preguntar a ciegas qué incluir.

## Plantilla HTML — estructura a poblar

La plantilla `reporte_competitivo_bancolombia.html` ya resuelve el chasis visual. La skill **adapta el contenido** a las secciones siguientes. No se debe rediseñar la plantilla — se debe poblar.

### Header
- **Título del reporte:** *Benchmark Competitivo — [Categoría / Decisión] — [Período]*.
- **Ventana de observación visible** (ej. "Ventana: últimos 12 meses · Q1 2026" — usando el badge de período de la plantilla).
- **Tag de confidencialidad** con render diferenciado por nivel:
  - **Interno** — tag gris claro.
  - **Confidencial** — tag amarillo (accent Bancolombia) o coral.
  - **Restringido** — tag negro con letras blancas.
- **Versión** si es cíclico (ej. "v3 · Edición Q1 2026").
- **Fecha de cierre** del análisis.

### Sidebar (orden recomendado de secciones)
1. Resumen ejecutivo
2. Encuadre y alcance
3. Metodología y fuentes
4. Hallazgos por dimensión (lectura horizontal)
5. Análisis por jugador (lectura vertical)
6. Anticipación competitiva *(solo si aplica)*
7. Retos para Bancolombia
8. Insights
9. Recomendaciones bisturí
10. Hipótesis abiertas (para investigación primaria)
11. Anexo — matriz completa, evidencia, log

### Cómo poblar cada sección con bloques de la plantilla

| Sección | Bloque(s) de la plantilla a usar |
|---|---|
| **Resumen ejecutivo** | KPI grid con 3–4 cifras núcleo + callout `co-insight` (amarillo) con la lectura central |
| **Encuadre y alcance** | Card simple con datos del encuadre, tabla de dimensiones |
| **Metodología y fuentes** | Tabla con tipos de fuente usados + nota sobre anonimización + tabla de fuentes aportadas por el usuario |
| **Hallazgos por dimensión** | Una `card` por dimensión con `co-insight`, `co-info`, badges (`b-hi`, `b-md`, `b-down`) y tablas comparativas |
| **Análisis por jugador** | `cg` (competitor cards) — una por jugador, encabezado con color (Bancolombia siempre primero) |
| **Anticipación competitiva** | `co-alert` (rojo) con la señal principal + tabla de señales con calor y verificación regulatoria + `co-info` con caminos regulatorios |
| **Retos para Bancolombia** | Cards con badges de criticidad (`b-hi` alta, `b-md` media, `b-st` baja) y horizonte; `co-alert` para retos críticos |
| **Insights** | `co-insight` (amarillo) por insight, con la anatomía formal expuesta (Hecho / Motivación / Tensión / Insight) y verbatims en bloque de cita |
| **Recomendaciones bisturí** | Tabla con columnas: Reto / Insight / Recomendación / Segmento / Canal / Producto / Mensaje / Dueño / Horizonte |
| **Hipótesis abiertas** | `co-info` (azul) listando hipótesis y método sugerido para validación primaria |
| **Anexo** | Tabla de la matriz completa + log de búsqueda + links al dossier de evidencia |

### Gráficos (Chart.js — ya cargado en la plantilla)
Producir gráficos solo cuando haya data cuantitativa que lo justifique:
- Comparativo de pricing / tasas → bar chart.
- Engagement relativo en redes → bar chart.
- Frecuencia de posteo por plataforma → stacked bar.
- Línea de tiempo de señales de anticipación → timeline simple.

No forzar gráficos si la dimensión es cualitativa. Mejor una buena tabla que un gráfico vacío.

## Reglas de marca Bancolombia (validar antes de cerrar)

| Regla | Cómo se valida en el HTML |
|---|---|
| **Amarillo siempre presente** | Al menos un `co-insight`, un `kpi` con accent o un badge amarillo en cada sección visible. |
| **Sin degradados** | No usar `linear-gradient` salvo el placeholder de imágenes vacías de la plantilla. Backgrounds planos. |
| **Negro CIB sobre blanco** | Títulos `h2` y `h3` en negro absoluto sobre fondo blanco. No invertir salvo header. |
| **Tipografía** | Inter (la plantilla la carga desde Google Fonts). Mantener consistencia con el reporte existente. |
| **Logo / header** | Respetar la altura `--header-h` y la jerarquía del header de la plantilla. |
| **Confidencialidad visible** | Tag `conf-tag` siempre presente en el header. |

## Pasos que debo ejecutar

### Paso 1 — Leer la plantilla y los entregables previos
- Leer la plantilla con `Read` para tener su estructura presente.
- Leer encuadre, plan, fuentes, levantamiento, social y análisis para tener todo el contenido.

### Paso 2 — Construir el esqueleto del reporte
Producir un HTML basado en la plantilla, con cada sección del sidebar creada y placeholders para el contenido. Mantener el chasis visual intacto.

### Paso 3 — Poblar contenido por sección
Recorrer las 11 secciones del sidebar (10 si no aplica anticipación) y poblar con los bloques correspondientes de la plantilla.

**Consideraciones específicas:**
- **Bancolombia siempre primero** en cualquier comparativo de jugadores (regla heredada de Fase 2).
- **Verbatims con anonimización del autor** preservada (regla heredada de Fase 4b social).
- **Insights con anatomía formal completa** — los cuatro componentes nombrados.
- **Recomendaciones ligadas a reto + insight** — no recomendaciones huérfanas.
- **Anticipación competitiva**, si aplica, con verificación regulatoria visible (no solo señal de redes).

### Paso 4 — Validar reglas de marca
Pasar el HTML por la lista de reglas de marca. Corregir si algo se rompió en la adaptación.

### Paso 5 — Generar Chart.js cuando aplique
Insertar gráficos solo donde hay data cuantitativa con valor narrativo. Usar la paleta accent del template (yellow / coral / teal / blue).

### Paso 6 — Construir la ficha de archivo
Documento markdown con metadatos para que el reporte sea recuperable por búsquedas futuras.

**Definir la ventana de vigencia y la fecha de refresh recomendado:**
- Si **one-off:** vigencia default **6 meses** desde el cierre, o hasta evento disruptivo (entrada de nuevo competidor, cambio regulatorio mayor, lanzamiento que altera el campo).
- Si **cíclico:** vigencia hasta la próxima edición (anual / semestral / trimestral). Marcar fecha estimada de la siguiente edición.
- **Anticipación competitiva:** vigencia más corta (3–4 meses) por la velocidad del entorno.

Si el benchmark es **continuación de una edición previa**, agregar un bloque de "Cambios respecto a la edición anterior" (qué jugadores entraron / salieron, qué dimensiones se agregaron, qué insights ganaron o perdieron vigencia).

### Paso 7 — Validar follow-ups
Revisar las hipótesis abiertas del análisis. Si alguna justifica investigación primaria, redactar la nota de derivación al flujo reactivo (`insights-intake`).

### Paso 8 — Archivo
- Guardar el HTML en `Comparacion vs competidores/entregas/<BMK-YYYY-NN>/reporte.html`.
- Guardar la ficha de archivo en `Comparacion vs competidores/entregas/<BMK-YYYY-NN>/archivo.md`.
- En la ficha, incluir links relativos a los entregables intermedios y al dossier de evidencia.

## Entregables

### Reporte HTML
Archivo: `Desktop/Gerencia Consumer Insights/Comparacion vs competidores/entregas/<BMK-ID>-<titulo-corto>/reporte.html`.

Construido sobre la plantilla, con las 10–11 secciones populadas y reglas de marca validadas.

### Ficha de archivo (metadatos)
Archivo: `…/entregas/<BMK-ID>-<titulo-corto>/archivo.md`.

```
FICHA DE ARCHIVO — BENCHMARK #BMK-YYYY-NN
════════════════════════════════════════
Título: [...]
Fecha de cierre: YYYY-MM-DD
Solicitante: [nombre / área / VP]
Tipo de origen: [Reactivo / Anticipación / Desprendimiento]
Decisión de negocio que alimentó:

CONFIDENCIALIDAD Y RECURRENCIA
─────────────────────────────────────────
Nivel de confidencialidad: [Interno / Confidencial / Restringido]
Tipo de ejercicio: [One-off / Cíclico]
  Si cíclico:
    - Cadencia: [Anual / Semestral / Trimestral / Otra: ___]
    - Versión: vN
    - Edición previa: BMK-...
    - Edición siguiente estimada: YYYY-MM
    - Cambios respecto a edición anterior: [...]

VENTANAS
─────────────────────────────────────────
Ventana de observación: [...]
Ventana de vigencia del reporte: [hasta YYYY-MM-DD / hasta próxima edición / hasta evento disruptivo]
Fecha de refresh recomendado: YYYY-MM-DD
Disparadores que adelantarían el refresh:
  - Entrada de nuevo competidor al mercado
  - Cambio regulatorio mayor (SFC, BRE-B, Open Finance)
  - Lanzamiento que altere el campo competitivo
  - Otros: ___

ALCANCE
─────────────────────────────────────────
Segmento: [...]
Categoría / dimensión del negocio: [...]
Geografía: [Colombia / Internacional / Ambos — mercados]

JUGADORES (Bancolombia + N)
─────────────────────────────────────────
- Bancolombia (ancla)
- [Competidor 1] — vehículo: [bancario / SEDPE / etc.]
- ...

DIMENSIONES COMPARADAS
─────────────────────────────────────────
- [...]

INSIGHTS CLAVE (texto corto)
─────────────────────────────────────────
- I1: [...]
- I2: [...]
- ...

RETOS PARA BANCOLOMBIA (texto corto)
─────────────────────────────────────────
- RT1 ([categoría], [criticidad]): [...]
- RT2 ([categoría], [criticidad]): [...]
- ...

RECOMENDACIONES BISTURÍ — TÍTULOS
─────────────────────────────────────────
- R1: [...]
- ...

FUENTES PRINCIPALES USADAS
─────────────────────────────────────────
- [...]

HIPÓTESIS ABIERTAS (para investigación primaria)
─────────────────────────────────────────
- [...] → derivable a insights-intake

TAGS PARA BÚSQUEDA
─────────────────────────────────────────
[segmento] [categoría] [jugadores principales] [dimensiones] [tipo: benchmark]

ENTREGABLES INTERMEDIOS (links relativos)
─────────────────────────────────────────
- Encuadre: ../../encuadres/BMK-YYYY-NN-...md
- Plan: ../../planes/BMK-YYYY-NN-...md
- Fuentes: ../../fuentes/BMK-YYYY-NN-...md
- Levantamiento desk: ../../levantamiento/BMK-YYYY-NN-...md
- Levantamiento social: ../../levantamiento/BMK-YYYY-NN-social.md
- Análisis: ../../analisis/BMK-YYYY-NN-...md
- Dossier de evidencia: ../../levantamiento/BMK-YYYY-NN/

VALIDACIONES DE CIERRE
─────────────────────────────────────────
[ ] Ventana de observación visible en el header del reporte
[ ] Tag de confidencialidad aplicado según nivel (Interno gris / Confidencial amarillo / Restringido negro)
[ ] Si es cíclico: versión y bloque de cambios vs edición previa visibles
[ ] Ventana de vigencia y fecha de refresh definidas en la ficha de archivo
[ ] Reglas de marca aplicadas (amarillo presente, sin degradados, Negro CIB sobre blanco, Inter)
[ ] Bancolombia primero en todo comparativo
[ ] Insights con anatomía formal completa
[ ] Recomendaciones ligadas a retos e insights
[ ] Anonimización de autores en verbatims preservada
[ ] Anticipación con verificación regulatoria (si aplica)
[ ] Hipótesis abiertas evaluadas para derivación a flujo reactivo
[ ] Ficha de archivo con metadatos completos
```

## Gate de salida
✅ Reporte HTML construido sobre la plantilla y validado contra reglas de marca, con ventana de observación visible y tag de confidencialidad por nivel + ficha de archivo con metadatos completos (incluyendo ventana de vigencia, fecha de refresh y disparadores de refresh anticipado) + si es cíclico, versión y delta vs edición previa + entregables intermedios linkeados + hipótesis abiertas evaluadas para derivación a `insights-intake` + carpeta `entregas/<BMK>/` cerrada.

## Next step
- Si hay hipótesis abiertas que requieran investigación primaria, abrir solicitud nueva con `insights-intake` referenciando este benchmark como antecedente.
- Si el sponsor pide presentación presencial complementaria, derivar al equipo el armado del deck — el reporte HTML es el artefacto maestro y queda como referencia permanente.
- Cierre formal del flujo de Benchmark Competitivo para esta solicitud.

## Referencias
- `Flujo_Benchmark_Competitivo.md` — Fase 6.
- Plantilla: `reporte_competitivo_bancolombia.html` (carpeta madre).
- `Filosofia_Consumer_Insights.md` — 5 filtros aplicados en Fase 5 quedan visibles en el reporte.
- Memoria: `reference_paleta_bancolombia.md` — paleta y reglas de marca.
- `Anatomia_Insights.md` — formato de insights expuestos.
