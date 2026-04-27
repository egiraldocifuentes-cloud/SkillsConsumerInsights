---
name: insights-informe
description: Construye el informe final de una investigación y la presentación ejecutiva, con executive summary, hallazgos por objetivo, insights estructurados como dolor→tensión→insight, contexto del banco durante el periodo (competencia, acciones propias, CX), recomendaciones accionables como bisturí con dueños asignados, y plan de seguimiento post-entrega. Archiva en el repositorio con metadatos para reuso. Usar después del análisis, o cuando el usuario diga "armar el informe final", "preparar el deck", "presentación para el sponsor", "cerrar el estudio", "entregar el informe".
---

# Skill: Informe final y entrega (Etapa 6 del flujo CI)

## Filosofía aplicada
El informe es el momento donde el equipo demuestra que construyó conocimiento accionable y estratégico — no que pasó el informe del aliado. **Cada insight del informe se presenta con la anatomía formal del equipo**: Hecho + Motivación + Tensión.

Reglas no negociables:
- No entregar solo el dato; entregar el **porqué del dato**.
- Cada insight debe estar estructurado en **Hecho + Motivación + Tensión** y escrito como frase densa que los entrelace (ver ejemplos en `Anatomia_Insights.md`).
- Cada insight debe venir con una **decisión concreta y un dueño**.
- De **escopeta a bisturí**: recomendaciones específicas, no genéricas.
- Cada slide/sección responde *"¿qué cambia en lo que hacemos después de esto?"*.

Leer obligatoriamente:
- `Anatomia_Insights.md`.
- `Filosofia_Consumer_Insights.md`.
- `Onboarding_Bancolombia_VP_Mercadeo.md`.

## Propósito
Comunicar hallazgos para **impulsar decisión**, archivar para reuso y cerrar el ciclo midiendo impacto post-entrega.

## Cuándo invocar
- Hay documento de hallazgos e insights (`ANA-*.md`).
- Hay que armar informe, executive summary o deck.
- Hay que cerrar y archivar.

## Entradas
1. **Hallazgos e insights** (`ANA-*.md`).
2. **Brief original**.
3. **Propuesta metodológica**.
4. **Reporte de campo**.
5. Formato esperado (informe largo / deck / ambos / dashboard).

## Pasos

### 6.1. Diseñar el informe final

Estructura obligatoria:

1. **Executive summary (1 página)**
   - Pregunta del estudio.
   - 3–5 hallazgos clave expresados como insights (no como datos).
   - 2–4 recomendaciones accionables.
   - Próximos pasos.

2. **Contexto del periodo** — crítico, diferencia al equipo:
   - Qué hacía Bancolombia durante el campo (campañas, cambios de producto, incidentes como caídas de canales).
   - Qué hacían los competidores (Grupo Aval, Grupo Bolívar/Davivienda/DAVIbank, BBVA, neobancos como Nubank/Lulo/Daviplata).
   - Qué pasaba en el consumidor/mercado.

3. **Contexto y objetivos del estudio** (del brief).

4. **Metodología** (resumen: enfoque, técnica, universo, N, error, fechas, aliado).

5. **Hallazgos por objetivo** — un bloque por objetivo con:
   - Hallazgo (descripción).
   - **Insight** presentado en **dos formatos** obligatorios:
     - (a) **Frase densa narrativa** que entrelaza los tres componentes (ver ejemplos en `Anatomia_Insights.md`, p. ej. el caso de clientes +65).
     - (b) **Descomposición anatómica** explícita: Hecho / Motivación / Tensión.
   - Evidencia (dato + verbatim).
   - Implicación.

6. **Confirmación/refutación de hipótesis del sponsor.**

7. **Insights transversales** no previstos en brief.

8. **Recomendaciones accionables — bisturí**:

   | Recomendación | Dueño sugerido | Impacto esperado | Plazo | Tipo |
   |---|---|---|---|---|
   | …  | … | … | … | Bisturí / Exploración / Medición futura |

9. **Próximos pasos propuestos.**

10. **Anexos**: cuestionario/guía, tablas, verbatims adicionales, cuotas, metodología detallada.

### 6.2. Deck ejecutivo (10–15 slides máx)

#### 6.2.1. Plantilla obligatoria — Bancolombia

**El deck SIEMPRE se construye a partir de:**
`Desktop/Gerencia Consumer Insights/templates/plantilla-deck-bancolombia.html`

Esta plantilla ya cumple Manual de Marca Bancolombia:
- Tipografía CIBFont Sans embebida (woff2 base64) con fallback a Open Sans + Arial.
- Paleta primaria Blanco + Negro CIB `#2C2A29` (no `#000000`).
- Paleta secundaria como acento: Amarillo Macondo `#FDDA24` (color de confianza, siempre presente cuando haya multicolor), Verde Andino `#00C389`, Azul Caribe `#59CBE8`, Rosa Flamenco `#F5B6CD`, Violeta Orquídea `#9063CD`, Naranja Alba `#FF7F41`.
- Sin degradados (`linear-gradient`/`radial-gradient` prohibidos por manual).
- Logo Bancolombia (SVG horizontal positivo) sobre fondo blanco en cada slide.
- 15 slides skeleton con la estructura del informe (S1-S15) y placeholders `{{NOMBRE}}`.

#### 6.2.2. Procedimiento

1. **Copiar la plantilla** al folder del estudio:
   `repositorio/<año>/<codigo-estudio>/<codigo>-deck.html`
2. **Reemplazar placeholders** `{{...}}` con el contenido del estudio (ver lista debajo).
3. **No introducir degradados** ni colores fuera de paleta. Si necesitas un color semántico de "alerta/wrong" usa Naranja Alba (no rojo).
4. **No usar all-caps en titulares** — sentence case (primera letra mayúscula). Los `s-label` y badges pequeños sí pueden ir en uppercase.
5. **Resaltar un único elemento por slide** — si varios elementos compiten al mismo nivel, ninguno destaca.
6. **Si falta un slide** (p. ej. solo hay 4 insights, no 6) → eliminar los slides sobrantes; no rellenar con contenido genérico.

#### 6.2.3. Estructura (S1–S15)

- S1: Portada — `{{TITULO_ESTUDIO}}`, sponsor, fecha, código.
- S2: Executive summary — pregunta + 3 hallazgos clave + 2 recomendaciones + próximos pasos.
- S3: Contexto del periodo (banco + competencia + consumidor + CX, 4 cards).
- S4: Contexto y objetivos del estudio (antecedentes, objetivo general, objetivos específicos, decisión).
- S5: Metodología (KPIs: N, error, cobertura, duración + cards: universo, aliado, cuotas, fechas).
- S6–11: Hallazgos + insights — un slide por insight con **frase densa** + **anatomía explícita Hecho/Motivación/Tensión** + evidencia (dato + verbatim) + implicación. Si solo hay 4 insights, dejar 4 slides; eliminar S10 y S11.
- S12: Recomendaciones bisturí (tabla con dueño, impacto, plazo, tipo).
- S13: Insights transversales no previstos en brief.
- S14: Próximos pasos + check-in 30-60 días.
- S15: Cierre + contacto.

**Regla de diseño:** cada slide responde *"¿qué cambia después de esta slide?"*. Si no, va a anexo.

### 6.3. Sesión de entrega

1. Presentación viva 30–60 min.
2. Espacio para preguntas e interpretación conjunta.
3. **Asignar dueños a recomendaciones** y fechas durante la sesión.
4. Documentar decisiones tomadas.

### 6.4. Publicación al repositorio

Archivar en `Desktop/Gerencia Consumer Insights/repositorio/<año>/<codigo-estudio>/` con:
- Informe (markdown + PDF si aplica).
- Deck.
- Brief original.
- Propuesta metodológica.
- Reporte de campo.
- Hallazgos e insights.
- Base o transcripciones (si política lo permite).
- **Metadatos (`metadata.md` o `.json`):**
  - Código, título, fecha, sponsor.
  - Segmento(s) (Personal 1-5MM / Plus 5-8MM / Plus Alto 8MM+ / Preferencial / Pyme / Empresas / Corporativo / Gobierno).
  - Marca(s) del grupo (Bancolombia / Nequi / Sufi / Wompi / Wenia / Tuya / Renting).
  - Metodología.
  - N muestra.
  - Aliado.
  - Tags (mínimo 5).
  - Insights clave.
  - Decisiones tomadas.

### 6.5. Seguimiento post-entrega

Agendar **check-in a 30–60 días** con sponsor para:
- Validar qué decisiones se tomaron.
- Medir impacto (KPI, cambio de estrategia, resultado).
- Alimentar aprendizaje del equipo.

Registrar en metadatos.

## Entregables

1. **Informe final** (markdown, PDF si aplica).
2. **Deck ejecutivo**.
3. **Tabla de recomendaciones con dueños y fechas**.
4. **Archivo en repositorio con metadatos.**
5. **Nota de seguimiento post-entrega.**

## Filtro de filosofía (antes de entregar)
- [ ] ¿Hay contexto del periodo? (no es solo el dato suelto)
- [ ] ¿Cada insight tiene los 3 componentes de la anatomía (Hecho + Motivación + Tensión)?
- [ ] ¿La motivación está nombrada con marco teórico (Maslow / Censydiam), no por intuición?
- [ ] ¿Cada insight está escrito como frase densa que entrelaza los tres?
- [ ] ¿Las recomendaciones son bisturí, no escopeta?
- [ ] ¿Hay dueños explícitos?
- [ ] ¿El sponsor puede tomar una decisión concreta después de leer el executive summary?

## Filtro de marca Bancolombia (deck)
- [ ] ¿El deck se construyó a partir de `templates/plantilla-deck-bancolombia.html`?
- [ ] ¿Cero degradados (`linear-gradient`/`radial-gradient`)?
- [ ] ¿Tipografía CIBFont Sans visible (no Inter/Quicksand/Arial fallback)?
- [ ] ¿Paleta solo Blanco + Negro CIB `#2C2A29` + 6 secundarios oficiales?
- [ ] ¿Amarillo Macondo presente en cualquier momento multicolor?
- [ ] ¿Logo Bancolombia sobre fondo blanco en cada slide?
- [ ] ¿Titulares en sentence case (no ALL CAPS)?
- [ ] ¿Cero placeholders `{{...}}` sin reemplazar?

## Gate de salida
✅ Entregado + presentado + dueños asignados + archivado con metadatos + seguimiento agendado + filtro de filosofía aprobado.

## Next step
Cerrar. Si surgen necesidades nuevas del informe → `insights-intake`.

## Referencias
- `Anatomia_Insights.md` — anatomía formal del insight + ejemplos del equipo.
- `Filosofia_Consumer_Insights.md`.
- `Flujo_Proceso_Consumer_Insights.md` (Etapa 6).
- `Onboarding_Bancolombia_VP_Mercadeo.md` — para contexto de banco, competidores, CX, stakeholders a incluir en la distribución.
- `templates/plantilla-deck-bancolombia.html` — plantilla obligatoria para el deck (ver §6.2.1).
- `~/Desktop/Manual de Marca Bancolombia/` — Manual de Marca oficial (paleta `BB_Paleta_RGB.ase`, logos `Logos/`, tipografía `Identidad visual/CIBFont Sans/`).
