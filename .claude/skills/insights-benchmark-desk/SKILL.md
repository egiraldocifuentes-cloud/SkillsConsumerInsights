---
name: insights-benchmark-desk
description: Ejecuta el desk research general de un benchmark competitivo (Fase 4a del flujo). Toma el plan de fuentes de Fase 3 y recolecta evidencia trazable para llenar la matriz comparativa: información de sitios web oficiales, apps, tiendas de aplicaciones, sitios de reseñas, reportes regulatorios (SFC, Asobancaria), prensa especializada y reportes de consultoras. Captura links, fechas, cifras con fuente y screenshots; mantiene log de búsqueda con queries anonimizadas; marca celdas no trianguladas y gaps de información. **No interpreta** — documenta. Usar después de `insights-benchmark-fuentes`. Para redes sociales y comunidades online, invocar en paralelo `insights-benchmark-social`.
---

# Skill: Desk research general de benchmark (Fase 4a del flujo)

## Filosofía aplicada
**En esta fase se documenta, no se interpreta.** La interpretación llega en Fase 5 con `insights-benchmark-analisis`. Mezclar análisis y levantamiento contamina la lectura: aparecen sesgos antes de tener la matriz completa.

Cada celda de la matriz tiene que tener fuente trazable. Si no hay fuente, no hay celda — se reporta el gap, no se inventa.

Leer `Flujo_Benchmark_Competitivo.md` (Fase 4) antes de ejecutar la skill.

## Propósito
Ejecutar el desk research siguiendo el plan de fuentes de Fase 3 y dejar la información cruda lista para análisis: matriz comparativa diligenciada + dossier de evidencia organizado por jugador + log de búsqueda.

## División del trabajo de levantamiento
Esta skill cubre fuentes "estructuradas y públicas":
- Sitios web oficiales y portales de inversionistas.
- Apps móviles y tiendas de aplicaciones (revisión y descarga de reviews).
- Sitios de reseñas y comparación.
- Reportes regulatorios (SFC, Asobancaria, Banco de la República, reguladores internacionales).
- Prensa especializada y analistas.
- Reportes de industria y consultoras.
- Documentos y enlaces aportados por el usuario en Fase 3.

Para **redes sociales corporativas, comunidades, foros y grupos online**, invocar en paralelo `insights-benchmark-social`. Las dos skills llenan distintas dimensiones de la misma matriz.

## Cuándo invocar
- Después de cerrar `insights-benchmark-fuentes`.
- Cuando hay que actualizar un benchmark previo con datos frescos sobre un jugador específico.

## Entradas que necesito
1. El **plan de fuentes cerrado** (`BMK-YYYY-NN-fuentes`).
2. La **matriz vacía** del plan de Fase 2.
3. Las **fuentes aportadas por el usuario** ya capturadas en Fase 3.

## Estilo conversacional
Trabajar en bloques verificables. Por cada bloque levantado, presentar al usuario un mini-resumen (qué se llenó, qué quedó como gap) antes de avanzar al siguiente. No vaciar la matriz completa de una sola pasada sin chequeo.

## Reglas de levantamiento

1. **Toda celda tiene fuente trazable.** Link directo + fecha de consulta + screenshot cuando aplique.
2. **Ventana de observación respetada.** Todo dato cuya fecha caiga fuera de la ventana definida en el encuadre se marca como **"contexto histórico — fuera de ventana"** y NO entra en celdas comparativas. Puede usarse como nota lateral si aporta entendimiento, pero no se cuenta como evidencia.
3. **Triangulación cuando aplique:** si una afirmación se sostiene en una sola fuente, marcarla como "no triangulada" en la celda.
4. **No interpretar.** Documentar el dato, no la implicación. Si aparece una hipótesis durante el levantamiento, anotarla en una sección aparte de "Lecturas tentativas" — no contaminar la celda.
5. **Anonimización en queries.** Toda búsqueda en lenguaje neutro, según las queries definidas en Fase 3. No mencionar Bancolombia ni Grupo Cibest en prompts a herramientas externas.
6. **Reportar gaps explícitamente.** Si una celda no tiene información pública dentro de la ventana, marcarla como "información no disponible en ventana" — no rellenarla con dato fuera de ventana.
7. **Aval consolidado.** Si el plan tiene "Grupo Aval", levantar información combinada de las marcas del holding y reportarla como conglomerado, no marca a marca.
8. **Internacional con contexto.** Para referentes internacionales, capturar también el contexto regulatorio o de mercado que distingue al país, porque eso será insumo para la traducción al contexto colombiano en Fase 5. Idioma: capturar URL y citas en idioma original (regla heredada de Fase 3).
9. **Marco regulatorio colombiano.** Cuando se levante información de competidores en Colombia, anotar el **vehículo de operación** del jugador (bancario / SEDPE / compañía de financiamiento / cross-border / sandbox / partnership). Detalle en `Flujo_Benchmark_Competitivo.md` sección 3.

## Pasos que debo ejecutar

### Paso 1 — Procesar fuentes aportadas por el usuario (prioritarias)
Si la Fase 3 capturó documentos o enlaces del usuario, empezar por ahí:
- Leer cada PDF o documento local con `Read`.
- Extraer datos relevantes con cita textual cuando aplique.
- Llenar las celdas de la matriz que esa fuente alimente.
- Registrar la fuente en el log de búsqueda como "aportada por usuario".

### Paso 2 — Levantamiento por jugador (recomendado por defecto)

Recorrer la matriz **jugador por jugador**, llenando todas sus dimensiones antes de pasar al siguiente. Esto da una visión integral por entidad y facilita la triangulación interna.

Para cada jugador:
1. Sitio oficial + portal de inversionistas → portafolio, propuesta declarada, performance corporativa.
2. App + tienda → CX, ratings, reviews, funcionalidades.
3. Sitios de reseñas → pricing y CX percibido.
4. Reportes regulatorios → cifras de mercado (cuando aplique al jugador).
5. Prensa y consultoras → movimientos estratégicos, lanzamientos, controversias.
6. Documentos aportados que apliquen.

**Modo alternativo — levantamiento por dimensión:** si el sponsor priorizó una dimensión (ej. pricing de hipoteca), recorrer la matriz dimensión por dimensión llenando esa columna para todos los jugadores antes de pasar a la siguiente.

### Paso 3 — Captura de evidencia
Por cada celda llenada:
- **Link** directo al sitio / documento.
- **Fecha de consulta** (la URL puede cambiar).
- **Screenshot** cuando la información sea visual (UX de app, post de redes, página de pricing) — guardar en `Comparacion vs competidores/levantamiento/<BMK-YYYY-NN>/<jugador>/`.
- **Cita textual o cifra** con fuente, no parafraseado vago.
- **Triangulación:** si hay segunda fuente que confirma, agregarla. Si no, marcar "no triangulada".

### Paso 4 — Log de búsqueda
Mantener un log con cada query ejecutada:
- Query exacta usada.
- Fuente / motor de búsqueda.
- Resultado útil obtenido (sí / no).
- Notas de hallazgos secundarios (cosas interesantes que no entraban en el plan pero pueden alimentar futuros benchmarks).

### Paso 5 — Lecturas tentativas (separadas)
Durante el levantamiento van apareciendo lecturas tentativas. Capturarlas en una sección aparte, **sin meterlas en la matriz**. Son insumo para Fase 5, no conclusiones. (Distinto de las "hipótesis abiertas" que produce la Fase 5 — esas son preguntas que requieren campo primario y se derivan a `insights-intake`.)

### Paso 6 — Cierre de la fase
- Validar que toda celda tiene fuente o está marcada como gap.
- Validar que el dossier de evidencia está organizado por jugador.
- Validar que el log de búsqueda está completo.
- Producir el entregable.

## Entregable

```
LEVANTAMIENTO DE BENCHMARK #BMK-YYYY-NN
════════════════════════════════════════
Plan de fuentes asociado: [BMK-YYYY-NN-fuentes]
Ventana de observación: [...]
Nivel de confidencialidad: [Interno / Confidencial / Restringido]
Modo de levantamiento: [Por jugador / Por dimensión]
Fecha de cierre del levantamiento:

MATRIZ DILIGENCIADA
─────────────────────────────────────────
| Jugador \ Dimensión | D1 | D2 | D3 (CX) | D4 | D5 | D6 |
|---|---|---|---|---|---|---|
| Bancolombia (ancla) | [dato + link + fecha] | ... | ... | ... | ... | ... |
| [Competidor 1] | [dato + link + fecha] | ... | ... | ... | ... | ... |
| [Competidor 2] | ... | ... | ... | ... | ... | ... |

Cada celda en formato:
  • Dato / hallazgo
  • Fuente: [nombre + URL] | Fecha: YYYY-MM-DD
  • Triangulación: [Sí — segunda fuente] / [No — fuente única]
  • Captura: [ruta del screenshot si aplica]

GAPS IDENTIFICADOS
─────────────────────────────────────────
| Jugador | Dimensión | Razón del gap |
|---|---|---|
| [Competidor X] | [Dimensión Y] | Información no disponible públicamente / requiere mystery shopping / requiere fuente paga |

LOG DE BÚSQUEDA
─────────────────────────────────────────
| # | Query (anonimizada) | Fuente / motor | Útil | Notas |
|---|---|---|---|---|
| 1 | "..." | Google / SFC / consultora | Sí / No | ... |

HIPÓTESIS EMERGENTES (insumo para Fase 5, no conclusiones)
─────────────────────────────────────────
- [Hipótesis tentativa 1]
- [Hipótesis tentativa 2]

REGLAS APLICADAS
─────────────────────────────────────────
[ ] Toda celda con fuente trazable o gap marcado
[ ] Datos fuera de ventana marcados como "contexto histórico" y excluidos de celdas comparativas
[ ] Anonimización aplicada en queries
[ ] Triangulación marcada por celda (sí / no)
[ ] Aval levantado como conglomerado
[ ] Capturas guardadas en /levantamiento/<BMK>/<jugador>/

DOSSIER DE EVIDENCIA
─────────────────────────────────────────
Carpeta: Comparacion vs competidores/levantamiento/<BMK-YYYY-NN>/
Estructura:
  /<jugador>/screenshots/
  /<jugador>/documentos/
  /<jugador>/notas.md

PRÓXIMO PASO
Próxima skill: insights-benchmark-analisis
(Si queda pendiente levantamiento de redes/comunidades: insights-benchmark-social)
```

Guardar el resumen en: `Desktop/Gerencia Consumer Insights/Comparacion vs competidores/levantamiento/<BMK-ID>-<titulo-corto>-levantamiento.md`.

## Gate de salida
✅ Matriz diligenciada con fuente por celda (o gap marcado) + dossier de evidencia organizado por jugador + log de búsqueda completo + hipótesis emergentes separadas + reglas aplicadas.

## Next step
- Si quedan dimensiones de **redes sociales / comunidades** por levantar, invocar `insights-benchmark-social`.
- Si la matriz está completa, continuar con `insights-benchmark-analisis` (Fase 5).

## Referencias
- `Flujo_Benchmark_Competitivo.md` — Fase 4 y reglas de levantamiento.
- Plan de fuentes (`BMK-YYYY-NN-fuentes`) — guía operativa de qué buscar dónde.
- Memoria: `feedback_anonimizacion_desk_research.md`, `feedback_competidores_grupo_aval.md`.
