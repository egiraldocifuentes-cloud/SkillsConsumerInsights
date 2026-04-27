# BITÁCORA — CONSTRUCCIÓN DEL SISTEMA DE CONSUMER INSIGHTS
## Registro de la sesión de trabajo con Claude para diseñar el sistema operativo del equipo

**Fecha:** Abril 2026
**Equipo:** Gerencia Consumer Insights — VP Mercadeo, Bancolombia / Grupo Cibest

---

## ÍNDICE

1. [Contexto y propósito](#1-contexto-y-propósito)
2. [Iteración 1 — Onboarding de Bancolombia](#2-iteración-1--onboarding-de-bancolombia)
3. [Iteración 2 — Correcciones al onboarding](#3-iteración-2--correcciones-al-onboarding)
4. [Iteración 3 — Flujo del proceso de Consumer Insights](#4-iteración-3--flujo-del-proceso-de-consumer-insights)
5. [Iteración 4 — Skills v1 (las 6 iniciales)](#5-iteración-4--skills-v1-las-6-iniciales)
6. [Iteración 5 — Sesión con el equipo: filosofía y robustecimiento](#6-iteración-5--sesión-con-el-equipo-filosofía-y-robustecimiento)
7. [Iteración 6 — Anatomía formal de los insights](#7-iteración-6--anatomía-formal-de-los-insights)
8. [Estado final del sistema](#8-estado-final-del-sistema)
9. [Memorias persistentes generadas](#9-memorias-persistentes-generadas)
10. [Próximos pasos sugeridos](#10-próximos-pasos-sugeridos)

---

## 1. CONTEXTO Y PROPÓSITO

El objetivo fue construir un **sistema operativo completo** para el equipo de Consumer Insights de Bancolombia, partiendo del entendimiento del banco hasta llegar a un set de skills automatizables que estandarizan el flujo de trabajo del área y refuerzan su filosofía estratégica.

La sesión avanzó por iteraciones — cada entrega fue retroalimentada con contexto interno del equipo, y cada ronda elevó el rigor del sistema:

```
Onboarding del banco
   ↓
Correcciones de hechos internos
   ↓
Flujo del proceso de investigación
   ↓
Skills v1 (operativas)
   ↓
Sesión con el equipo → filosofía + skills v2 (estratégicas)
   ↓
Anatomía formal del insight → skills v3 (con teoría del equipo)
```

---

## 2. ITERACIÓN 1 — ONBOARDING DE BANCOLOMBIA

### Pedido
Documento de onboarding para alguien nuevo en la VP de Mercadeo. Debía cubrir:
- Tipos de clientes que atiende el banco.
- Portafolio de productos y servicios en Colombia.
- Competidores (banca retail y banca empresas/jurídica).
- Percepción de los consumidores colombianos sobre la marca.
- Gaps y fortalezas frente a neobancos.
- Stakeholders del banco en el país.
- Apoyado en fuentes confiables.

### Investigación
Búsqueda en fuentes oficiales y especializadas: SFC, Asobancaria, Merco, Portafolio, La República, Bloomberg Línea, El Colombiano, Infobae, Valora Analitik, sitios oficiales del Grupo Cibest, Fiduciaria Bancolombia, Wikipedia institucional.

### Entregable
**`Onboarding_Bancolombia_VP_Mercadeo.md`**

Contenido inicial:
- Estructura del Grupo Cibest (mayo 2025).
- Posición de mercado (cartera comercial 34,8%, libre inversión 23,16%, cuota total ~31,6%).
- Segmentos de clientes (banca de personas y banca de empresas).
- Portafolio completo por persona natural y jurídica.
- Competidores agrupados por tipo.
- Reputación (Merco 2025, ranking #1 por 10 años).
- Gaps y fortalezas frente a neobancos.
- Stakeholders del banco.
- 35+ fuentes referenciadas.

---

## 3. ITERACIÓN 2 — CORRECCIONES AL ONBOARDING

El equipo aportó correcciones críticas que las fuentes públicas no reflejan o desactualizan:

### Correcciones aplicadas
1. **Banistmo fue vendido en diciembre 2025** a Inversiones Cuscatlán por USD 1.418 M. Ya no hace parte del Grupo Cibest.
2. **Segmentación de Banca de Personas por ingresos:**
   - Personal: 1–5 MM
   - Personal Plus: 5–8 MM
   - Plus Alto / Preferencial: 8 MM en adelante
3. **Sufi** es un NIT y marca propia del Grupo Cibest (no estaba mapeado). Crédito de movilidad, educativo, consumo y seguros.
4. **Nequi NO es un canal digital de Bancolombia** — es un NIT y marca independiente del Grupo Cibest.
5. **Ahorro a la Mano** ya no hace parte del portafolio de Bancolombia.
6. **Competidores Grupo Aval** deben analizarse como conglomerado (Banco de Bogotá, Occidente, Popular, AV Villas, dale!) sin perder mirada por marca. Igual lectura para Grupo Bolívar (Davivienda, DAVIbank, Daviplata).
7. **Ausencia crítica:** la **experiencia del cliente** (canales físicos y digitales) debía ser un eje explícito, no un supuesto.

### Entregable
**`Onboarding_Bancolombia_VP_Mercadeo.md` versión 2.0** con:
- Estructura del grupo actualizada (sin Banistmo).
- Segmentos con rangos correctos.
- Sufi mapeado en estructura, portafolio y experiencia.
- Nequi reclasificado como marca/NIT independiente.
- Competidores agrupados por conglomerado (Grupo Aval, Grupo Bolívar) con mirada consolidada e individual.
- **Nueva sección 5 — Experiencia del Cliente (CX)** con canales físicos, digitales, incidentes (caídas masivas feb-2026), experiencia diferenciada por marca del grupo, gaps y fortalezas frente a neobancos.

### Memorias persistentes generadas en esta iteración
- Rol del usuario (Consumer Insights Bancolombia/Cibest).
- Estructura del Grupo Cibest (Nequi y Sufi son NITs propios, Banistmo vendido, Ahorro a la Mano descontinuado).
- Segmentación oficial por ingresos.
- Regla de análisis competitivo por conglomerado.
- CX como eje obligatorio.

---

## 4. ITERACIÓN 3 — FLUJO DEL PROCESO DE CONSUMER INSIGHTS

### Pedido
Formalizar el flujo operativo del área con 6 etapas:
1. Necesidad/solicitud de stakeholder.
2. Brief.
3. Definición de metodología (cuali / cuanti / híbrida).
4. Ejecución (campo).
5. Análisis de data.
6. Informe final y entrega.

### Entregable
**`Flujo_Proceso_Consumer_Insights.md`**

Contenido:
- Diagrama visual del flujo con 6 etapas y *gates* (puntos de control).
- Cada etapa documentada con: objetivo, entradas, actividades clave, salidas, roles, gate de salida, buenas prácticas.
- Gobierno del proceso (tiempos estándar por tipo de estudio, criterios de calidad, roles del equipo, cumplimiento legal — Ley 1581, SFC).
- Anexos con plantillas: formulario de solicitud, brief, propuesta metodológica, checklist de gates.

---

## 5. ITERACIÓN 4 — SKILLS v1 (LAS 6 INICIALES)

### Pedido
Crear las skills (slash commands) para ejecutar el flujo completo, con resumen de cada una.

### Entregables
6 skills instaladas en `.claude/skills/`:

| Skill | Etapa | Función |
|---|---|---|
| `/insights-intake` | 1 | Recepción y triage de solicitudes |
| `/insights-brief` | 2 | Construcción del brief |
| `/insights-metodologia` | 3 | Diseño metodológico (cuali/cuanti/híbrido) |
| `/insights-campo` | 4 | Cuestionario, piloto, controles, reporte de campo |
| `/insights-analisis` | 5 | Análisis de data y construcción de insights |
| `/insights-informe` | 6 | Informe final, deck, archivado |

Cada skill: YAML frontmatter, propósito, cuándo invocar, pasos, entregables, gate de salida, next step, referencias.

---

## 6. ITERACIÓN 5 — SESIÓN CON EL EQUIPO: FILOSOFÍA Y ROBUSTECIMIENTO

### Insumo
Conversación interna del equipo de Consumer Insights con su gerente, donde explicaron los principios que los diferencian. Las ideas centrales que se extrajeron:

### Principios clave del equipo

> *"No somos mensajeros."* No hacen copy-paste. No llaman al aliado para que presente directamente al área solicitante. Estudian lo que el aliado entrega y **lo conectan con el negocio del banco**.

> *"Pensamos estratégicamente, no operativamente."* Transforman data en decisiones, no entregan data.

> *"Conectamos puntos — sinapsis."* Un insight es la conexión de puntos dispersos.

> *"Anticiparse al mercado — ver más allá."* Trascender lo que la VP de Mercadeo necesita hoy.

> *"Oído, ojos y sensibilidad hacia afuera."* Escuchar, ver, observar y traducir al banco.

> *"Leer entre líneas."* No quedarse en la superficie.

> *"De escopeta a bisturí."* Marketing dirigido, no masivo.

### Framework conversacional Dolor → Tensión → Insight

Aparece en la conversación con un ejemplo magistral:

| Nivel | Ejemplo |
|---|---|
| Dolor | "¿Quién me ayuda con el pago a proveedores?" |
| Tensión | "Estoy perdiendo tiempo y dinero haciendo este proceso" |
| Insight | "Necesito tiempo para que mi empresa vaya al siguiente nivel — ¿quién me libera ese espacio?" |

Impacto en marketing:
- Mensaje operativo (dolor): *"Le tengo esta herramienta para que haga el pago"*.
- Mensaje estratégico (insight): *"Le tengo esta herramienta para que siga creciendo"*.

### Modalidades de trabajo

- **Reactivo:** solicitudes de stakeholders (flujo documentado).
- **Proactivo:** scouting de tendencias.
  - "Rastreamos. Los discutimos en equipo. Y en equipo seleccionamos el tema."
  - Persona encargada desarrolla, hace informe, entrega.
- **Recurrente estratégico:** estudio de marca semestral.
  - Brand Equity + Brand Contribution.
  - Todos los segmentos: personas, PYME, empresas, corporativo.
  - Aliado externo (Kantar) entrega data; **el equipo construye el porqué**.
  - Considera contexto del periodo: competencia, acciones propias, experiencia del cliente, caídas de canales.

### Retos permanentes del equipo
- Tiempo (el constante).
- Costos.
- Acceso al público objetivo.

### Robustecimiento de las skills

Resultado: las 6 skills se actualizaron y se crearon 2 nuevas.

#### Cambios en las 6 skills existentes:

- **`/insights-intake`** — distinción reactivo/proactivo, cuestionamiento activo si no hay decisión clara, filtro de 5 criterios de filosofía.
- **`/insights-brief`** — bloque explícito Dolor→Tensión→Insight hipotético, regla de oro, estilo conversacional sparring.
- **`/insights-metodologia`** — análisis explícito de los 3 retos, criterios para elegir aliado, regla "el aliado entrega data, el equipo construye insight".
- **`/insights-campo`** — instrumento que captura tensión (no solo dolor), blind study para marcas propias.
- **`/insights-analisis`** — tabla de 5 pasos para pasar de dolor a insight, contexto del periodo obligatorio, sparring de Claude con preguntas.
- **`/insights-informe`** — sección obligatoria de contexto del periodo, recomendaciones categorizadas como bisturí.

#### Skills nuevas:

- **`/insights-tendencias`** — flujo proactivo: rastrear → discutir → seleccionar (5 criterios) → profundizar → entregar. "Oído afuera".
- **`/insights-brand-tracking`** — recurrente estratégico: estudio de marca semestral con Brand Equity + Brand Contribution en todos los segmentos, contexto del periodo, comparativo Grupo Aval / Grupo Bolívar / neobancos / marcas del grupo.

### Documento de filosofía
**`Filosofia_Consumer_Insights.md`** — brújula del equipo con principios, framework, criterios de calidad, modalidades de trabajo y retos permanentes. Todas las skills la referencian.

---

## 7. ITERACIÓN 6 — ANATOMÍA FORMAL DE LOS INSIGHTS

### Insumo
Documento del equipo: **`Anatomía de los insights.docx`** — teoría formal sobre cómo construir insights.

### Hallazgo central
El equipo tiene una formulación teórica más sofisticada que la conversacional:

> **INSIGHT = HECHO + MOTIVACIÓN + TENSIÓN**

### Definiciones formales del documento original

**¿Qué es un insight?**
> *"Una verdad profunda o epifanía que proporciona una comprensión de la naturaleza real de las cosas, más allá de lo que puede parecer obvio. Un insight va más allá: es una verdad profunda que conecta con una motivación o necesidad humana, y que genera una fricción o tensión que espera ser resuelta."*

**¿Qué NO es un insight?**
- Un dato, un verbatim, una señal, una métrica.
- Un hallazgo, una conclusión, una tendencia.
- Una creencia, un juicio, una opinión.

Todo lo anterior puede ser **materia prima** del insight, pero no es el insight.

### Componentes

| Componente | Definición | Cómo se identifica |
|---|---|---|
| **Hecho** | Verdad objetiva y verificable | Datos cuantitativos, métricas, tendencias, verbatims, hallazgos |
| **Motivación** | Disparador humano detrás del comportamiento | Pirámide de Maslow + Modelo Censydiam (Freud + Jung + McClelland + Alderfer) |
| **Tensión** | Fricción o barrera que choca con la motivación | Observación directa, conversaciones con consumidores |

### Los 3 ejemplos del equipo

**1. Clientes +65 de Bancolombia**
- *Hecho:* representan 10% de la base; tienen Brand Power significativamente más alto que jóvenes 18–25.
- *Motivación:* relación construida en el tiempo — gracias a Bancolombia compraron casa, carro, educación. Pertenencia.
- *Tensión:* dependencia de canales físicos (solo 7% transacciones digitales son financieras) y solo 4% son preferenciales. Los digitales no suman valor.

**2. Fiducuenta como caja fuerte de fin de semana**
- *Hecho:* 5 de cada 10 clientes con cuenta de ahorros tienen Fiducuenta activa; mueven saldos solo el fin de semana — pico los viernes.
- *Motivación:* esconder el dinero **de sí mismos** para evitar gastos impulsivos. Autocontrol.
- *Tensión:* usan un producto de ahorro a largo plazo como mecanismo anti-impulso, lejos de su finalidad. Y no le ven valor a Bolsillos en la App, diseñado para esto.

**3. Selección Colombia — el fútbol que une**
- *Hecho:* 4 de cada 10 mujeres en Colombia son aficionadas al fútbol.
- *Motivación:* buscar un grupo con el cual identificarse. Pertenencia.
- *Tensión:* el amor al club a veces divide — pero cuando juega la Selección, todos se nos olvida de qué equipo somos hinchas.

### Robustecimiento aplicado a las skills

Se reemplazó el framework conversacional (Dolor→Tensión→Insight) por la anatomía formal (Hecho + Motivación + Tensión) como **estándar de trabajo**, manteniendo el conversacional como herramienta pedagógica para explicar a stakeholders.

#### Cambios en las 5 skills constructoras de insight:

- **`/insights-brief`** — bloque "Anatomía del Insight Hipotético" con 4 campos. Preguntas piden nombrar la motivación con Maslow/Censydiam.
- **`/insights-analisis`** — tabla de 6 pasos (Hecho → Motivación → Tensión → Conexión afuera-adentro → Insight → Implicación). Filtro anatómico: si no se nombran los 3 componentes, no es insight.
- **`/insights-informe`** — cada insight en dos formatos obligatorios: frase densa + descomposición anatómica. Filtro valida marco teórico para la motivación.
- **`/insights-tendencias`** — interpretación de tendencias en formato anatómico.
- **`/insights-brand-tracking`** — hallazgos de salud de marca traducidos a insight formal. Referencia explícita al ejemplo +65 como aplicable directamente.

#### Las 3 skills restantes (intake, metodología, campo) — ajustadas:
Referencian la anatomía con función específica: intake evalúa si la solicitud permite construir insight; metodología garantiza que el diseño levante los tres componentes; campo asegura que las preguntas capturen evidencia para los tres.

### Documento creado
**`Anatomia_Insights.md`** — síntesis del documento original del equipo, accesible para que las skills lo referencien. Incluye definición, lista de "no-insights", la fórmula, modelos teóricos para motivación, los 3 ejemplos descompuestos, y la relación con el framework conversacional.

### Filosofía actualizada
Sección 3 de `Filosofia_Consumer_Insights.md` ahora presenta el framework formal como estándar y el conversacional como complemento. Tabla de equivalencias incluida.

---

## 8. ESTADO FINAL DEL SISTEMA

### 📁 Documentos en la carpeta de trabajo

```
Desktop/Gerencia Consumer Insights/
├── Onboarding_Bancolombia_VP_Mercadeo.md      [v2.0 — banco, segmentos, competencia, CX]
├── Flujo_Proceso_Consumer_Insights.md         [6 etapas con plantillas y gates]
├── Filosofia_Consumer_Insights.md             [principios + framework + filtros]
├── Anatomia_Insights.md                       [teoría formal del equipo]
├── Anatomía de los insights.docx              [original del equipo]
├── Bitacora_Construccion_Sistema_CI.md        [este documento]
└── .claude/
    └── skills/
        ├── insights-intake/SKILL.md           [Etapa 1 — triage reactivo/proactivo]
        ├── insights-brief/SKILL.md            [Etapa 2 — brief con anatomía formal]
        ├── insights-metodologia/SKILL.md      [Etapa 3 — metodología + aliado]
        ├── insights-campo/SKILL.md            [Etapa 4 — campo + QA]
        ├── insights-analisis/SKILL.md         [Etapa 5 — anatomía + sinapsis]
        ├── insights-informe/SKILL.md          [Etapa 6 — informe con contexto]
        ├── insights-tendencias/SKILL.md       [Proactivo — oído afuera]
        └── insights-brand-tracking/SKILL.md   [Recurrente estratégico — semestral]
```

### 🧩 Las 8 skills disponibles

| Skill | Trigger principal | Salida |
|---|---|---|
| `/insights-intake` | Llega solicitud o se detecta señal | Solicitud triada con decisión |
| `/insights-brief` | Hay solicitud abierta | Brief firmable con anatomía hipotética |
| `/insights-metodologia` | Brief firmado | Propuesta metodológica con aliado |
| `/insights-campo` | Metodología aprobada | Instrumento + reporte de campo |
| `/insights-analisis` | Data lista | Insights con anatomía formal |
| `/insights-informe` | Insights construidos | Informe + deck + archivo en repositorio |
| `/insights-tendencias` | Señal externa proactiva | Informe de tendencia con anatomía |
| `/insights-brand-tracking` | Llega data del aliado semestral | Informe de salud de marca con contexto |

### 🧠 Lógica del sistema

```
Stakeholder pide algo (reactivo)         Equipo detecta señal (proactivo)         Aliado entrega data semestral
         ↓                                          ↓                                          ↓
   /insights-intake                       /insights-tendencias                     /insights-brand-tracking
         ↓
   /insights-brief
         ↓
   /insights-metodologia
         ↓
   /insights-campo
         ↓
   /insights-analisis  ←── filtro anatómico (Hecho + Motivación + Tensión)
         ↓
   /insights-informe
         ↓
   Check-in 30–60 días con sponsor
```

### 🎯 Filtros transversales

Cualquier entregable del equipo debe pasar:

**Filtro de filosofía (5 criterios):**
- ¿Conecta puntos o solo describe?
- ¿Llega a insight o se queda en hecho/dolor?
- ¿Habilita acción/decisión?
- ¿Hay mirada externa explicando interna?
- ¿Es bisturí, no escopeta?

**Filtro anatómico (3 componentes):**
- ¿Tiene Hecho explícito (dato verificable)?
- ¿Tiene Motivación explícita (con marco teórico)?
- ¿Tiene Tensión explícita (no asumida)?

**Filtro de calidad del insight (4 criterios):**
- Relevante / Novedoso / Accionable / Soportado.

---

## 9. MEMORIAS PERSISTENTES GENERADAS

Estas memorias se cargan automáticamente en futuras conversaciones para mantener continuidad:

| Memoria | Tipo | Contenido |
|---|---|---|
| User role | user | Trabaja en CI Bancolombia/Cibest, conocimiento interno |
| Estructura Grupo Cibest | project | Nequi y Sufi son NITs; Banistmo vendido; Ahorro a la Mano descontinuado |
| Segmentación Personas | project | Personal 1–5MM, Plus 5–8MM, Plus Alto 8MM+ |
| Competidores Grupo Aval | feedback | Mirada de conglomerado para Aval, Bolívar, Gilinski |
| CX como eje obligatorio | feedback | Todo documento estratégico debe cubrir CX |
| Filosofía del equipo | project | Conectores estratégicos, no mensajeros; modalidades reactivo/proactivo/recurrente |
| Anatomía formal del insight | project | Hecho + Motivación + Tensión; modelos Maslow/Censydiam; ejemplos |

---

## 10. PRÓXIMOS PASOS SUGERIDOS

### Validación inmediata
- **Probar `/insights-analisis` con un caso real** — por ejemplo, un hallazgo del próximo brand tracking semestral, para validar que el guiado conduce a insight formal con los tres componentes nombrados.
- **Probar `/insights-tendencias` con una señal real** detectada por el equipo en redes o prensa.
- **Probar `/insights-brief` con la siguiente solicitud que llegue** y validar que el bloque de anatomía hipotética funciona.

### Ajustes finos posibles
- Si el equipo tiene plantillas internas diferentes a las usadas (formularios de solicitud propios, templates de brief de marca, decks corporativos), las skills pueden incorporarlas literalmente.
- Las skills incluyen ejemplos de preguntas conversacionales — el equipo puede pulirlas con frases reales que usen en kickoffs.

### Capacidades adicionales potenciales
- **`/insights-repositorio`** — para buscar estudios pasados antes de abrir nuevos (sería el complemento natural de la Etapa 1, donde se valida si la pregunta ya tiene respuesta).
- **`/insights-nps`** — flujo dedicado para NPS relacional y transaccional (frecuencia distinta al brand tracking).
- **`/insights-social-listening`** — flujo proactivo específico para señales de redes y conversación digital.
- **Skill de coaching pedagógico** — para enseñar el framework anatómico a stakeholders que pidan estudios pero no entiendan la diferencia entre dolor e insight.

### Mantenimiento del sistema
- Cuando salga el siguiente brand tracking semestral, registrarlo en el repositorio con metadatos para que aparezca en futuros triages.
- Cuando el Grupo Cibest cambie estructura (ventas, adquisiciones, marcas nuevas), actualizar el onboarding y la memoria de estructura.
- Cuando el equipo identifique un nuevo principio o regla recurrente, agregarla como memoria de feedback para que aplique en sesiones futuras.

---

## ANEXO — DECISIONES CLAVE DE LA SESIÓN

| Decisión | Razón |
|---|---|
| Skills al nivel de proyecto, no global | Son específicas para Consumer Insights de Bancolombia; no aplican a otros proyectos |
| Skills en español, no inglés | Coherencia con la operación del equipo y con el contenido de la documentación |
| Anatomía formal como estándar, conversacional como complemento | El framework formal es la teoría del equipo; el conversacional es útil pero secundario |
| Documentos `.md` en raíz, no en carpetas internas | Accesibilidad y referenciado simple desde las skills |
| Mantener `Anatomía de los insights.docx` original | Documento formal del equipo, no se reemplaza, se sintetiza |
| Memorias en proyecto separado, no en CLAUDE.md raíz | Las memorias persisten entre conversaciones del mismo proyecto sin contaminar otras carpetas |
| Documento de bitácora separado | Útil para nuevos miembros del equipo que necesiten entender cómo se construyó el sistema |

---

*Documento de bitácora de la sesión. Útil como referencia histórica, material de inducción para nuevos integrantes del equipo, y punto de partida si se desea evolucionar el sistema en el futuro.*
