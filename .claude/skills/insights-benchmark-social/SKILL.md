---
name: insights-benchmark-social
description: Ejecuta el levantamiento del benchmark en redes sociales corporativas y comunidades online (Fase 4b del flujo). Cubre LinkedIn, X, Instagram, TikTok, YouTube y Facebook como canales corporativos de cada jugador, y Reddit, Quora, grupos públicos de Facebook, comunidades de Telegram / Discord, foros financieros y blogs especializados como espacios de voz no filtrada del cliente. Captura narrativa, tono, frecuencia y engagement de las marcas; verbatims y fricciones espontáneas de los usuarios; señales tempranas de aterrizaje de nuevos competidores en Colombia (cuentas que despiertan, contrataciones locales, partnerships anunciados). Aplica el marco regulatorio colombiano (SFC, Banco de la República, FOGAFIN, BRE-B, Open Finance, vehículos de operación: bancario / SEDPE / compañía de financiamiento / cross-border) como lente obligatorio para interpretar tanto la comunicación de los competidores actuales como las señales de los nuevos entrantes. Aplica reglas de anonimización en queries, captura de evidencia con screenshots fechados, y resguardo de identidad de usuarios no públicos. Usar en paralelo a `insights-benchmark-desk` cuando el plan de fuentes incluye redes y comunidades.
---

# Skill: Desk research en redes y comunidades online (Fase 4b del flujo)

## Filosofía aplicada
En este flujo las redes y comunidades cumplen un rol distinto al sitio web oficial:
- Las **cuentas corporativas** muestran lo que la marca quiere proyectar — narrativa, tono, prioridades.
- Las **comunidades y foros** muestran lo que el cliente realmente vive — fricciones, comparaciones espontáneas, expectativas.

Las dos lecturas son complementarias y obligatorias. Una sin la otra contamina el benchmark: o leemos solo el discurso de marca, o solo el ruido del cliente sin contexto.

**En esta fase se documenta, no se interpreta.** La interpretación llega en Fase 5.

Leer `Flujo_Benchmark_Competitivo.md` (Fase 4) antes de ejecutar la skill.

## Propósito
Levantar la información de redes sociales corporativas y comunidades online prevista en el plan de fuentes (Fase 3), llenar las celdas correspondientes de la matriz comparativa con evidencia trazable, y capturar verbatims y señales tempranas en formato reusable.

## Cuándo invocar
- En paralelo a `insights-benchmark-desk` cuando el plan de fuentes incluye dimensiones que se alimentan de redes / comunidades (típicamente: comunicación, posicionamiento, CX percibida, anticipación competitiva).
- Cuando el sponsor pide específicamente "lectura social" o "qué dice la gente" sobre un jugador.
- Cuando el origen del benchmark es **anticipación competitiva** — las redes son el termómetro más temprano de un aterrizaje.

## Entradas que necesito
1. El **plan de fuentes cerrado** (`BMK-YYYY-NN-fuentes`) — específicamente, qué dimensiones se asignaron a redes / comunidades.
2. La lista de jugadores del plan, con sus handles oficiales si ya están identificados.
3. Comunidades, cuentas o voceros que el usuario haya aportado en Fase 3.

## Lente regulatorio aplicado a la lectura social

El marco regulatorio colombiano canónico (entes reguladores + vehículos de operación + implicaciones generales) vive en `Flujo_Benchmark_Competitivo.md` **sección 3**. Esta skill no lo duplica — lo aplica.

### Cómo se aplica el lente en cada bloque del levantamiento social

1. **Por cada jugador (Bloque A)**, anotar el **vehículo bajo el cual opera (o pretende operar) en Colombia** — bancario / SEDPE / compañía de financiamiento / cooperativa / comisionista / fiduciaria / cross-border / sandbox / partnership / no autorizado aún. Campo obligatorio en la matriz.

2. **Por cada lectura de comunicación (Bloque A)**, aplicar lectura regulatoria: ¿está dentro de lo permitido?, ¿usa lenguaje de producto que su licencia no soporta? (típico ejemplo: SEDPE comunicando "crédito directo"), ¿hay tensión visible con publicidad regulada SFC?, ¿menciona BRE-B o Open Finance?

3. **Por cada señal de anticipación (Bloque C)**, verificar el camino regulatorio: contrastar la señal de redes contra registros públicos — comunicados / autorizaciones SFC, sociedades en Cámara de Comercio, prensa especializada. Una señal social fuerte sin sustento regulatorio se marca como **"ruido" o "PR temprano"**, no como aterrizaje inminente. El "calor" de la señal se calibra con esa verificación.

4. **Por cada fricción de cliente (Bloque B)**, distinguir si la queja se ancla en una **restricción regulatoria** (ej. límites SEDPE, requisitos de identificación, reportes UIAF) o en una **falla de servicio**. Esa distinción es clave para Fase 5.

## Reglas de levantamiento

1. **Anonimización en queries y prompts.** Toda búsqueda en redes y prompts a herramientas de IA externas se redacta en lenguaje neutro. No mencionar Bancolombia ni Grupo Cibest como origen del análisis.

2. **Ventana de observación respetada.** Posts, hilos, verbatims y señales fechados fuera de la ventana del encuadre se marcan como **"contexto histórico"** y no entran como evidencia. Excepción explícita: en **anticipación competitiva**, se permite usar referencias históricas externas (ej. cómo el mismo jugador entró a otro mercado años atrás) como contexto proyectado, etiquetadas como tal.

3. **Resguardo de identidad de usuarios no públicos.** En comunidades (Reddit, foros, grupos de Facebook), no capturar el nombre real ni el username del usuario que escribe. Capturar el verbatim, la fecha, la comunidad y la URL — pero anonimizar al autor. Excepción: voceros públicos identificados (analistas, periodistas, influencers financieros con perfil público).

4. **Toda evidencia con screenshot.** Las URLs de redes se rompen, los posts se borran, los hilos se editan. Cada captura usada como evidencia se guarda en local con fecha en el nombre del archivo.

5. **Triangulación entre canales.** Una afirmación sobre tono o narrativa de una marca se sostiene en al menos dos plataformas (ej. LinkedIn + Instagram), no en una sola. Una afirmación sobre fricciones de cliente se sostiene en al menos dos comunidades distintas o un patrón claro de repetición.

6. **No tomar trolling como insight.** En comunidades hay ruido, sarcasmo y polarización. Marcar verbatims que parezcan trolling y no contarlos para construir patrones.

7. **Aval consolidado.** Lectura social del Grupo Aval se hace mirando las cuentas y comunidades de las marcas del holding y reportando como conglomerado.

## Estilo conversacional
Trabajar en bloques verificables, igual que `insights-benchmark-desk`. Por cada jugador o cada plataforma cubierta, presentar un mini-resumen al usuario (qué se llenó, qué quedó pendiente) antes de avanzar.

## Bloque A — Cuentas corporativas

### Plataformas y qué leer en cada una

| Plataforma | Qué se lee | Para qué dimensiones sirve |
|---|---|---|
| **LinkedIn** | Narrativa B2B, comunicación corporativa, posts de liderazgo, contrataciones, partnerships | Posicionamiento, comunicación, anticipación competitiva |
| **X (Twitter)** | Tono real-time, atención al cliente, manejo de crisis, frecuencia de posteo, voceros | Comunicación, CX (servicio en redes), reputación |
| **Instagram** | Narrativa visual, segmentos a los que apela, campañas activas, colaboraciones | Comunicación, posicionamiento, segmento |
| **TikTok** | Apuesta a Gen Z, educación financiera, viralidad, voceros internos | Comunicación, posicionamiento joven |
| **YouTube** | Contenido largo, anuncios, testimonios, tutoriales de producto | Comunicación, propuesta de valor |
| **Facebook** | Cobertura masiva en segmentos populares y regiones, pauta visible | Comunicación, segmento masivo |

### Qué capturar por jugador (mínimo)

- **Handle oficial** + plataformas activas + plataformas inactivas o abandonadas.
- **Vehículo de operación en Colombia** (bancario / SEDPE / compañía de financiamiento / cross-border / partnership / no autorizado aún) y referencia regulatoria que lo soporta.
- **Frecuencia de posteo** (posts/semana en los últimos 30 días).
- **Tipos de contenido dominantes** (educativo / promocional / institucional / humano / crisis).
- **Engagement promedio** (likes / comentarios / vistas — escala relativa, no absoluta).
- **Tono dominante** (formal / cercano / aspiracional / didáctico / irreverente).
- **Voceros visibles** (si hay liderazgo personal posteando).
- **Campañas activas** en el período del benchmark.
- **Tensión regulatoria visible** (si la comunicación roza límites SFC, si usa lenguaje de producto que su licencia no soporta, si menciona BRE-B / Open Finance).
- **3–5 capturas de posts representativos** por plataforma activa.

## Bloque B — Comunidades, foros y grupos online

### Espacios típicos

| Espacio | Qué se obtiene | Notas |
|---|---|---|
| **Reddit — r/Colombia, r/personalfinance, r/finanzas, r/argentina** | Comparaciones espontáneas entre bancos, fricciones reales, hilos largos sobre productos | Buscar el nombre del jugador; ordenar por "top" del último año |
| **Grupos públicos de Facebook** (finanzas personales, emprendedores, segmentos urbanos) | Voz menos técnica, problemas cotidianos, quejas, recomendaciones | Captura con cuidado de privacidad |
| **Quora en español** | Preguntas comparativas, respuestas largas | Menos activo que Reddit pero con contenido útil |
| **Foros financieros (Rankia, blogs especializados)** | Análisis de inversionistas retail, comparativos de productos | Útil para pricing y propuesta de inversión |
| **Comunidades de Telegram / Discord** (cripto, trading, finanzas) | Voz nativa digital, primeras menciones de nuevos jugadores | Documentar canal y permisos de captura |
| **Comentarios en YouTube** | Reacción cruda a anuncios o tutoriales | Especialmente valioso para CX percibida |
| **Reseñas en App Store / Google Play** | Quejas y elogios estructurados, ordenables por "más útiles" o "más recientes" | Cuenta como comunidad por la dinámica de respuesta |

### Qué capturar por comunidad

- **Verbatims relevantes**: cita textual + fecha + URL + nombre de la comunidad. Autor anonimizado salvo que sea figura pública.
- **Patrones repetidos** (ej. la misma queja aparece en 5 hilos distintos).
- **Comparaciones espontáneas** ("yo me cambié de X a Y porque…") — son oro para el insight.
- **Volumen estimado** de menciones del jugador en el período.
- **Sentimiento dominante** marcado conservadoramente (positivo / mixto / negativo / neutro).

## Bloque C — Anticipación competitiva en redes

Si el encuadre marcó **anticipación competitiva**, ejecutar un sub-levantamiento dirigido a detectar señales tempranas:

- **Cuentas localizadas que despiertan** (ej. handle "@nubankco" pasa de inactivo a posteando, o aparece "@xbankcolombia" sin lanzamiento público).
- **Ofertas de empleo en LinkedIn** del jugador buscando talento en Colombia.
- **Posts de liderazgo** mencionando Colombia como mercado de interés.
- **Partnerships anunciados** con jugadores locales (fintechs, retailers, telcos).
- **Domain registrations / trademarks** mencionados en prensa o redes.
- **Conversaciones espontáneas** en comunidades sobre la próxima entrada de X.

Documentar cada señal con: fecha, fuente, captura, y nivel estimado de "calor" (frío / tibio / caliente / inminente).

**Verificación regulatoria obligatoria por señal:** contrastar la señal de redes contra registros públicos para identificar el camino regulatorio:
- ¿Hay autorización o solicitud visible en la **SFC** (comunicados, listados públicos)?
- ¿Hay sociedad constituida en **Cámara de Comercio** (Colombia)?
- ¿Hay un **partnership** con entidad local ya autorizada?
- ¿Está usando un esquema **cross-border** o **sandbox regulatorio**?

Una señal social fuerte sin sustento regulatorio se marca como "ruido" o "PR temprano", no como aterrizaje inminente. El "calor" de la señal se calibra con esa verificación.

## Pasos que debo ejecutar

### Paso 1 — Procesar fuentes sociales aportadas por el usuario
Si la Fase 3 capturó cuentas, comunidades, posts o voceros específicos, empezar por ahí. Esos espacios son insumo prioritario.

### Paso 2 — Bloque A: cuentas corporativas
Recorrer plataforma por plataforma para cada jugador, capturando lo definido en el bloque A. Llenar las celdas de comunicación / posicionamiento / CX (servicio en redes) en la matriz.

### Paso 3 — Bloque B: comunidades y foros
Buscar cada jugador en las comunidades relevantes. Capturar verbatims y patrones, anonimizando autores. Llenar las celdas de CX percibida, pricing percibido y posicionamiento espontáneo.

### Paso 4 — Bloque C: anticipación competitiva (si aplica)
Ejecutar el sub-levantamiento de señales tempranas. Llenar la celda / sección de anticipación.

### Paso 5 — Captura y organización de evidencia
Guardar todas las capturas en `Comparacion vs competidores/levantamiento/<BMK-YYYY-NN>/<jugador>/social/`, separadas por subcarpeta `corporativas/` (Bloque A) y `comunidades/` (Bloque B).

### Paso 6 — Log de búsqueda
Mantener log con cada query / búsqueda ejecutada, plataforma, resultado útil sí/no.

### Paso 7 — Lecturas tentativas
Capturar lecturas tentativas en sección aparte, no en las celdas. Son insumo para Fase 5, no conclusiones. (Distinto de las "hipótesis abiertas" que produce la Fase 5 y se derivan a investigación primaria.)

### Paso 8 — Cierre
Validar que toda celda asignada a redes / comunidades tiene fuente (o gap marcado). Producir el entregable.

## Entregable

```
LEVANTAMIENTO SOCIAL #BMK-YYYY-NN
════════════════════════════════════════
Plan de fuentes asociado: [BMK-YYYY-NN-fuentes]
Ventana de observación: [...]
Nivel de confidencialidad: [Interno / Confidencial / Restringido]
Modo: [Estándar / Con sub-levantamiento de anticipación competitiva]
Fecha de cierre:

BLOQUE A — CUENTAS CORPORATIVAS
─────────────────────────────────────────
| Jugador | Vehículo de operación en CO | Plataformas activas | Frecuencia | Tipo de contenido dominante | Tono | Engagement relativo | Voceros visibles | Campañas activas | Tensión regulatoria visible |
|---|---|---|---|---|---|---|---|---|---|
| Bancolombia (ancla) | Establecimiento bancario | ... | ... | ... | ... | ... | ... | ... | — |
| [Competidor 1] | [bancario / SEDPE / cross-border / etc.] | ... | ... | ... | ... | ... | ... | ... | ... |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |

Capturas: /levantamiento/<BMK>/<jugador>/social/corporativas/

BLOQUE B — COMUNIDADES Y FOROS
─────────────────────────────────────────
| Jugador | Comunidades cubiertas | Volumen relativo de menciones | Sentimiento dominante | Patrones repetidos | Verbatims clave (ID) |
|---|---|---|---|---|---|
| Bancolombia (ancla) | ... | ... | ... | ... | V01, V02, V03 |
| [Competidor 1] | ... | ... | ... | ... | V04, V05 |
| ... | ... | ... | ... | ... | ... |

VERBATIMS CAPTURADOS (autores anonimizados)
| ID | Verbatim (cita textual) | Comunidad | Fecha | Tema |
|---|---|---|---|---|
| V01 | "..." | r/Colombia | YYYY-MM-DD | CX / pricing / comparación |
| ... | ... | ... | ... | ... |

Capturas: /levantamiento/<BMK>/<jugador>/social/comunidades/

BLOQUE C — SEÑALES DE ANTICIPACIÓN (si aplica)
─────────────────────────────────────────
| # | Señal | Fuente / plataforma | Fecha | Nivel de calor | Camino regulatorio detectado | Verificación SFC / Cámara | Captura |
|---|---|---|---|---|---|---|---|
| 1 | [ej. "@xbankco" empezó a postear el 12-feb] | LinkedIn / X | YYYY-MM-DD | Tibio / Caliente / Inminente | [Adquisición / Nueva licencia / SEDPE / Sandbox / Partnership / Cross-border / No identificado] | [link a comunicado SFC / sociedad en Cámara / "no encontrado"] | [ruta] |

GAPS IDENTIFICADOS
─────────────────────────────────────────
| Jugador | Bloque / dimensión | Razón del gap |
|---|---|---|

LOG DE BÚSQUEDA
─────────────────────────────────────────
| # | Query / búsqueda (anonimizada) | Plataforma | Útil | Notas |

LECTURAS TENTATIVAS (insumo para Fase 5)
─────────────────────────────────────────
- [...]

REGLAS APLICADAS
─────────────────────────────────────────
[ ] Anonimización en queries
[ ] Ventana de observación respetada (material fuera de ventana marcado como contexto histórico)
[ ] Identidad de usuarios no públicos resguardada
[ ] Toda evidencia con captura local fechada
[ ] Triangulación marcada (mínimo 2 plataformas o 2 comunidades por afirmación)
[ ] Trolling marcado y excluido de patrones
[ ] Aval levantado como conglomerado (si aplica)
[ ] Lente regulatorio aplicado: vehículo de operación documentado por jugador
[ ] Señales de anticipación verificadas contra SFC / Cámara de Comercio

PRÓXIMO PASO
Próxima skill: insights-benchmark-analisis
```

Guardar el resumen en: `Desktop/Gerencia Consumer Insights/Comparacion vs competidores/levantamiento/<BMK-ID>-<titulo-corto>-social.md`.

## Gate de salida
✅ Bloque A (corporativas) y Bloque B (comunidades) cubiertos para todos los jugadores asignados a redes + Bloque C levantado si el origen es anticipación + lente regulatorio aplicado (vehículo de operación documentado por jugador, señales de anticipación verificadas con SFC / Cámara) + verbatims anonimizados + capturas guardadas + reglas aplicadas.

## Next step
- Cuando `insights-benchmark-desk` y `insights-benchmark-social` estén ambas cerradas y la matriz esté completa, continuar con `insights-benchmark-analisis` (Fase 5).

## Referencias
- `Flujo_Benchmark_Competitivo.md` — Fase 4 y reglas transversales.
- Plan de fuentes (`BMK-YYYY-NN-fuentes`) — qué dimensiones se asignaron a redes y comunidades.
- Memoria: `feedback_anonimizacion_desk_research.md`, `feedback_competidores_grupo_aval.md`, `feedback_incluir_experiencia_cliente.md`.
