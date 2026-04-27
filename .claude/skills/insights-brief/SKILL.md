---
name: insights-brief
description: Construye el brief de investigación formal a partir de una solicitud ya triada. Toma una necesidad del stakeholder y la transforma en un documento de alineación con antecedentes, objetivo general, objetivos específicos, hipótesis, público, decisión, entregables, timing, presupuesto y restricciones. Aplica el framework Dolor→Tensión→Insight para definir bien la pregunta central del estudio. Usar después de insights-intake, o cuando el usuario diga "armar el brief", "redactar el brief", "estructurar el brief de esta solicitud".
---

# Skill: Construcción del brief (Etapa 2 del flujo CI)

## Filosofía aplicada
El brief es el documento donde el equipo **garantiza que va a construir un insight, no a entregar un dato**. Si el brief no tiene clara la decisión estratégica y no estructura el insight hipotético con la anatomía formal del equipo (**Hecho + Motivación + Tensión = Insight**), es un brief de mensajero — y eso no sale del equipo.

Leer obligatoriamente:
- `Anatomia_Insights.md` — marco teórico formal (Hecho + Motivación + Tensión).
- `Filosofia_Consumer_Insights.md` — principios operativos.
- `Onboarding_Bancolombia_VP_Mercadeo.md` — contexto del banco.

## Propósito
Transformar una solicitud triada en un **brief firmable** que asegure que sponsor, equipo de Insights y (si aplica) proveedor tienen el mismo entendimiento — y que el estudio está orientado a construir insight, no a recolectar información.

## Cuándo invocar
- El usuario pide "armar un brief".
- Ya existe un archivo de solicitud (`SOL-*.md`) y el triage dijo "abrir brief".
- El sponsor quiere formalizar una investigación.

## Estilo conversacional
Claude debe **guiar el ejercicio con preguntas**. El equipo prefiere que Claude les haga preguntas progresivas que vayan clarificando el brief, no que escriba el brief de un tiro en lenguaje corporativo. Hacer preguntas como:
- *"¿Cuál es la decisión que este estudio va a habilitar? Si no la puedes nombrar en una frase, todavía no tenemos brief."*
- *"¿Qué crees hoy que va a pasar? Eso es tu hipótesis — es diferente a la pregunta."*
- *"¿Qué HECHO motiva este estudio? ¿Qué MOTIVACIÓN humana sospechas detrás? ¿Qué TENSIÓN chocaría con esa motivación?"*
- *"¿Con qué modelo psicológico (Maslow, Censydiam) podríamos nombrar la motivación? ¿Pertenencia, autocontrol, estima, seguridad, reconocimiento, logro?"*

## Entradas que debo leer/pedir
1. **Archivo de solicitud triada** (`SOL-*.md`).
2. **Notas de la reunión de kickoff** con el sponsor (si existen).
3. Agenda de kickoff si falta información.

## Pasos que debo ejecutar

1. Leer la solicitud y extraer lo capturado.
2. **Identificar vacíos** en los 11 bloques del brief; pedirlos al usuario concentrados.
3. **Aplicar la regla de oro:** *"esta investigación habilitará la decisión X"*. Si no se puede llenar, devolver al usuario a afinar con el sponsor.
4. **Aplicar la anatomía formal del insight** al objetivo (ver `Anatomia_Insights.md`):
   - **Hecho hipotético:** qué dato/indicador/verbatim vamos a poner bajo la lupa.
   - **Motivación sospechada:** qué necesidad humana está detrás (nombrarla con Maslow o Censydiam — pertenencia, autocontrol, estima, seguridad, reconocimiento, logro, afiliación, poder).
   - **Tensión sospechada:** qué contradicción estorba la motivación.
   - **Insight hipotético:** síntesis narrativa.
   El objetivo general del brief debe apuntar a **revelar o validar el insight**, no a describir el hecho.
5. **Depurar objetivos difusos** ("entender mejor al cliente") → reformular como preguntas con respuesta concreta.
6. **Separar hipótesis del sponsor** (lo que cree que va a encontrar) de **preguntas de investigación** (lo que debe responder la data).
7. **Entregables esperados** explícitos (informe, deck, dashboard, workshop).
8. **Restricciones legales y regulatorias** — Ley 1581, SFC, marca.
9. **Identificar segmento exacto** según segmentación oficial de Bancolombia (Personal 1–5MM, Plus 5–8MM, Plus Alto 8MM+, Preferencial, Pyme, Empresas, Corporativo, Gobierno) y marca del grupo (Bancolombia, Nequi, Sufi, Wompi, Wenia, Tuya, Renting).
10. Redactar el brief y entregarlo para validación.

## Entregable

```
BRIEF DE INVESTIGACIÓN
────────────────────────────────────────────────
Título del estudio:
Sponsor:
Responsable de Insights:
Fecha:
Solicitud asociada:

1. ANTECEDENTES Y CONTEXTO
   (Qué está pasando en el negocio/mercado que motiva este estudio)

2. PROBLEMA / OPORTUNIDAD
   (En una frase, qué decisión pendiente existe)

3. ANATOMÍA DEL INSIGHT HIPOTÉTICO (Hecho + Motivación + Tensión)
   Hecho (verdad objetiva de partida — dato, métrica, verbatim):
   Motivación (disparador humano — nombrarla con Maslow/Censydiam):
   Tensión (fricción que choca con la motivación):
   Insight hipotético (síntesis narrativa):

4. OBJETIVO GENERAL
   (Pregunta principal que el estudio responderá — debe atacar al menos la tensión)

5. OBJETIVOS ESPECÍFICOS
   5.1.
   5.2.
   5.3.
   (Cada uno debe ser una pregunta concreta, no un tema)

6. HIPÓTESIS DE PARTIDA
   (Lo que el sponsor cree hoy — para contrastar)

7. PÚBLICO OBJETIVO / UNIVERSO
   Segmento(s) de banca:
   Marca(s) del grupo:
   Región / edad / género / relación con la marca:

8. DECISIÓN QUE HABILITARÁ LA INVESTIGACIÓN
   (Regla de oro — si no se puede llenar, no hay brief)

9. ENTREGABLES ESPERADOS

10. TIMING

11. PRESUPUESTO DISPONIBLE

12. RESTRICCIONES
    (Legales — Ley 1581 / SFC, de marca, de stakeholders)

────────────────────────────────────────────────
FILTRO DE FILOSOFÍA
[ ] El brief apunta a insight, no a dato
[ ] Conecta afuera (mercado/consumidor) con adentro (banco)
[ ] La decisión es concreta y accionable
[ ] No es escopeta (objetivos enfocados, no todo a la vez)

Firmas:
Sponsor ____________________
Consumer Insights ____________________
```

Guardar en `Desktop/Gerencia Consumer Insights/briefs/BRIEF-YYYY-MM-DD-<titulo-corto>.md`.

## Gate de salida
✅ 12 bloques completos + regla de oro cumplida + filtro de filosofía aprobado + sponsor listo para firmar.

Si no pasa el gate, **NO avanzar a Etapa 3**.

## Next step
Invocar `insights-metodologia` con el brief firmado.

## Referencias
- `Anatomia_Insights.md` — framework formal Hecho + Motivación + Tensión.
- `Filosofia_Consumer_Insights.md` — principios operativos del equipo.
- `Flujo_Proceso_Consumer_Insights.md` (Etapa 2).
- `Onboarding_Bancolombia_VP_Mercadeo.md` — segmentos oficiales y marcas del grupo.
