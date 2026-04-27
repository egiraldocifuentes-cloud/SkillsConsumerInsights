---
name: insights-benchmark-encuadre
description: Convierte una solicitud de comparación competitiva en un mini-brief de benchmark (Fase 1 del flujo de Benchmark Competitivo). Verifica que la pregunta sea efectivamente un benchmark — no investigación primaria, no scouting de tendencias, no data interna pura — y produce la ficha de encuadre con la decisión de negocio a alimentar, segmento, categoría, geografía, ventana de observación del mercado, nivel de confidencialidad (Interno / Confidencial / Restringido), tipo de ejercicio (one-off / cíclico), profundidad esperada, restricciones y estimación de esfuerzo del flujo. Estos inputs obligatorios gobiernan todo el flujo. Usar cuando llega una solicitud que pida "comparar Bancolombia con…", "qué hacen los competidores en X", "benchmark de Y", "cómo está nuestra propuesta vs…", o cuando el equipo detecte una señal de posible entrada de un nuevo competidor al mercado financiero colombiano y quiera anticipar la respuesta.
---

# Skill: Encuadre de benchmark competitivo (Fase 1 del flujo)

## Filosofía aplicada
Antes de mirar competidores, hay que entender **qué decisión del banco va a alimentar el ejercicio**. Un benchmark sin decisión asociada termina siendo una lista de cosas que hacen otros — escopeta, no bisturí. La gerencia no es mensajera. Si la solicitud no habilita una decisión estratégica, se devuelve.

Leer `Flujo_Benchmark_Competitivo.md` (carpeta `Comparacion vs competidores/`) y `Filosofia_Consumer_Insights.md` antes de ejecutar esta skill, al menos la primera vez de cada sesión.

## Propósito
Convertir una solicitud de comparación competitiva en una ficha de encuadre de 1–2 páginas que permita arrancar la Fase 2 (definición de jugadores y dimensiones) con claridad sobre **qué se compara y para qué**.

## Cuándo invocar
- Llega una solicitud explícita: "haz un benchmark de…", "compara Bancolombia con…", "qué hacen los neobancos en X", "cómo nos vemos frente a Y".
- Se detecta una **señal de posible entrada de un nuevo competidor** al mercado colombiano (ej. neobanco extranjero registrando dominio, abriendo oficina, contratando talento local) y se quiere preparar la respuesta antes de que llegue.
- Después de `insights-intake`, cuando el triage clasifica la solicitud como desk research competitivo y no como investigación primaria.

## Estilo conversacional
Guiar con preguntas, no esperar una descripción completa. Si el usuario describe la solicitud en forma libre:
1. Leer e identificar lo que ya está dicho.
2. Hacer preguntas concentradas en 1–2 bloques (no una a una).
3. Cuestionar si es necesario — si falta la decisión de negocio, decirlo explícitamente.

## Verificación previa (gate de entrada)
Antes de armar el encuadre, validar que esta es la skill correcta. Si la respuesta a alguna de estas es SÍ, **derivar al flujo correspondiente y cerrar esta skill**:

| Pregunta de descarte | Derivar a |
|---|---|
| ¿La pregunta requiere consultar consumidores (focus, IDIs, encuesta cuantitativa)? | `insights-intake` → flujo reactivo estándar |
| ¿La pregunta nace de una señal cultural amplia, no de una comparación entre jugadores definidos? | `insights-tendencias` |
| ¿Se puede responder con data interna pura (CRM, transaccional, NPS interno)? | Data analytics / BI — no es benchmark |

Solo si la pregunta sobrevive los tres filtros, continuar.

## Entradas que debo pedir al usuario

### Información de origen
1. **Solicitante / detector** (nombre y área/VP).
2. **Tipo de origen:**
   - Reactivo (solicitud de stakeholder).
   - Anticipación competitiva (señal de posible entrada de nuevo competidor a Colombia).
   - Desprendimiento de otra investigación previa.
3. **Fecha requerida** y **criticidad** (alta / media / baja).

### Encuadre del benchmark
4. **Decisión de negocio** que alimentará el benchmark — *¿qué va a hacer el sponsor con el resultado?*
5. **Segmento** del banco: Personas (Personal 1–5MM / Plus 5–8MM / Plus Alto 8MM+ / Preferencial), Pyme, Empresas, Corporativo, Gobierno; o marcas del grupo (Bancolombia, Nequi, Sufi, Wompi, Wenia, Tuya, Renting).
6. **Categoría / producto / dimensión** del negocio: tarjetas, hipoteca, app, pricing, comunicación, sostenibilidad, onboarding, CX, etc.
7. **Geografía:** Colombia / Internacional / Ambos. Si Internacional, qué mercados de referencia se proponen y por qué.
8. **Nivel de profundidad esperado:** panorámico (muchos jugadores, poco detalle) vs profundo (pocos jugadores, alto detalle).
9. **Restricciones:** tiempo, alcance, sensibilidad, presupuesto.
10. **Estudios previos o reportes existentes** que el sponsor conoce sobre el tema.

### Inputs que gobiernan el flujo (obligatorios)
11. **Ventana de observación del mercado** — el período del cual se observará a los jugadores. Opciones típicas:
    - Últimos N meses (ej. 6, 12, 18, 24).
    - Trimestre / semestre / año específico (ej. Q1 2026, S2 2025).
    - Desde un evento clave (ej. desde la salida de Scotiabank en dic-2025; desde el lanzamiento de DAVIbank).
    - Snapshot puntual (foto del mercado al día de hoy — válido para pricing, portafolio).
    - Para **anticipación competitiva:** ventana corta hacia atrás (señales recientes — 3–6 meses) + horizonte proyectado hacia adelante (cuándo se espera el aterrizaje).
12. **Nivel de confidencialidad:**
    - **Interno** — gerencia + VPs implicadas. Default cuando es benchmark reactivo sobre dimensiones públicas.
    - **Confidencial** — sponsor + selectos del banco. Default cuando hay material aportado por el sponsor o conclusiones sensibles.
    - **Restringido** — Presidencia / Comité Ejecutivo. Para alto impacto reputacional o estratégico.
    - **Anticipación competitiva → mínimo Confidencial.**
13. **Tipo de ejercicio:**
    - **One-off** — responde a una decisión puntual.
    - **Cíclico** — anual / semestral / trimestral. Si es cíclico: ¿qué cadencia?, ¿es nueva edición o continuación de una serie existente? (si continuación, capturar referencia a la edición anterior).

## Pasos que debo ejecutar

1. **Leer el input** y extraer lo que ya viene descrito.
2. **Aplicar verificación previa** (gate de entrada). Si no aplica, derivar y cerrar.
3. **Preguntar de forma concentrada** lo que falte.
4. **Cuestionar la decisión de negocio** explícitamente. Si el sponsor pide "comparar por comparar", devolver con: *"¿qué decisión vas a tomar con esto?"* No somos mensajeros.
5. **Validar coherencia interna:** segmento + categoría + geografía deben ser consistentes (ej. "hipoteca para Pyme en Brasil" requiere justificación clara).
6. **Validar coherencia decisión ↔ ventana de observación.** La ventana debe ser proporcional a la decisión: una decisión de campaña Q3 2026 con ventana de "últimos 5 años" probablemente está sobre-dimensionada; una decisión estratégica con ventana de "últimos 30 días" probablemente es insuficiente. Si hay desbalance, devolver al sponsor.
7. **Asignación por defecto de confidencialidad si no se especifica:**
   - Si origen = Anticipación competitiva → **mínimo Confidencial**.
   - Si la solicitud toca pricing detallado, posicionamiento estratégico o decisiones de portafolio → **Confidencial**.
   - Para benchmarks de comunicación pública, sostenibilidad, lectura de redes → **Interno**.
8. **Marcar reglas heredadas que aplican:**
   - Si entran competidores de Grupo Aval → leer como conglomerado.
   - Si la geografía incluye internacional → traducir al contexto colombiano antes de recomendar.
   - CX entra como dimensión obligatoria en Fase 2.
   - Anonimización en queries externas (lenguaje neutro, no mencionar Bancolombia).
9. **Estimar esfuerzo del flujo y validar contra la fecha requerida.** Usar la siguiente tabla orientativa como punto de partida y ajustar por complejidad real:

   | Alcance | Esfuerzo orientativo |
   |---|---|
   | 3 dimensiones × Bancolombia + 3 competidores · solo Colombia · sin social profundo | **1.5–2 semanas** |
   | 5 dimensiones × Bancolombia + 4 competidores · Colombia + 1–2 referentes internacionales · social estándar | **3–4 semanas** |
   | 5–7 dimensiones × Bancolombia + 6 competidores · pricing cuantitativo amplio · social profundo | **5–6 semanas** |
   | Anticipación competitiva con verificación regulatoria + sub-levantamiento social | **+1 semana adicional** |
   | Cíclico con comparación contra edición previa | **−0.5 semana** (matriz y jugadores parcialmente reusables) |

   Si la fecha requerida no encaja con el esfuerzo estimado, **devolver al sponsor** con dos opciones explícitas: ajustar alcance (menos jugadores / menos dimensiones / sin social profundo) o ajustar fecha. No comprometer escopeta para cumplir un plazo.

10. **Producir la ficha de encuadre.**

## Entregable

```
ENCUADRE DE BENCHMARK #BMK-YYYY-NN
════════════════════════════════════════
Solicitante / detector: [nombre / área / VP]
Tipo de origen: [ ] Reactivo  [ ] Anticipación competitiva  [ ] Desprendimiento
Fecha de solicitud:
Fecha requerida:
Criticidad: [Alta / Media / Baja]

VERIFICACIÓN DE FLUJO (gate de entrada)
─────────────────────────────────────────
[ ] No requiere data primaria con consumidores
[ ] No es señal cultural amplia (no es scouting de tendencias)
[ ] No es data interna pura (no es BI)
→ Si pasa los 3 filtros, continúa este flujo.

ENCUADRE
─────────────────────────────────────────
1. Decisión de negocio que alimentará
2. Segmento del banco
3. Categoría / producto / dimensión
4. Geografía (Colombia / Internacional / Ambos)
   - Mercados de referencia internacional propuestos:
5. Nivel de profundidad (panorámico / profundo)
6. Restricciones (tiempo, alcance, sensibilidad, presupuesto)
7. Estudios previos conocidos

INPUTS QUE GOBIERNAN EL FLUJO
─────────────────────────────────────────
8. Ventana de observación del mercado:
   [ ] Últimos N meses (N = ___)
   [ ] Trimestre / semestre / año específico (___)
   [ ] Desde evento clave (___)
   [ ] Snapshot al día de hoy
   [ ] Anticipación: ventana hacia atrás (___ meses) + horizonte proyectado (___ meses)
   Justificación de la ventana elegida:

9. Nivel de confidencialidad:
   [ ] Interno
   [ ] Confidencial
   [ ] Restringido
   Razón:

10. Tipo de ejercicio:
    [ ] One-off
    [ ] Cíclico — cadencia: [ ] Anual [ ] Semestral [ ] Trimestral [ ] Otra: ___
    Si es cíclico y existe edición previa: referencia BMK-...

ESTIMACIÓN DE ESFUERZO
─────────────────────────────────────────
Esfuerzo estimado del flujo: ___ semanas
Fecha requerida por el sponsor: YYYY-MM-DD
¿Encaja? [ ] Sí  [ ] No — Ajuste acordado: [reducir alcance / mover fecha / otro: ___]

REGLAS HEREDADAS A APLICAR EN FASES SIGUIENTES
─────────────────────────────────────────
[ ] Aval se lee como conglomerado (si aplica)
[ ] Internacional se traduce al contexto colombiano
[ ] CX entra como dimensión obligatoria en Fase 2
[ ] Anonimización en queries externas

CRITERIOS DE CALIDAD (preview)
─────────────────────────────────────────
- ¿La decisión de negocio es clara y accionable?
- ¿El segmento + categoría + geografía es coherente?
- ¿Hay suficiente alcance para construir bisturí, no escopeta?

PRÓXIMO PASO
Responsable sugerido:
Próxima skill: insights-benchmark-plan
```

Guardar en: `Desktop/Gerencia Consumer Insights/Comparacion vs competidores/encuadres/<BMK-ID>-<titulo-corto>-encuadre.md`.

Convención de ID: `BMK-YYYY-NN` (correlativo dentro del año). Detalle en `Flujo_Benchmark_Competitivo.md` sección 8.

## Gate de salida
✅ Encuadre cerrado con: decisión de negocio explícita + verificación de flujo aprobada + segmento/categoría/geografía coherentes + **ventana de observación definida y coherente con la decisión** + **nivel de confidencialidad asignado** + **tipo de ejercicio (one-off / cíclico) declarado** + **estimación de esfuerzo validada contra fecha requerida** + reglas heredadas marcadas + responsable asignado.

## Next step
- Continuar con `insights-benchmark-plan` (Fase 2).
- Si durante el encuadre se descubre que la pregunta sí requiere campo primario, derivar a `insights-intake` y cerrar.

## Referencias
- `Flujo_Benchmark_Competitivo.md` — flujo completo y principios transversales.
- `Filosofia_Consumer_Insights.md` — marco del equipo y 5 filtros de calidad.
- `Onboarding_Bancolombia_VP_Mercadeo.md` — segmentos oficiales, marcas del grupo, mapa competitivo.
- Memoria: `feedback_competidores_grupo_aval.md`, `feedback_anonimizacion_desk_research.md`, `feedback_incluir_experiencia_cliente.md`.
