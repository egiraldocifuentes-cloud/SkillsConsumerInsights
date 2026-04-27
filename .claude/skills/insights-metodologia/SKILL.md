---
name: insights-metodologia
description: Diseña la propuesta metodológica para una investigación — decide entre cualitativo, cuantitativo o híbrido, selecciona técnicas específicas (IDIs, focus groups, CAWI, CATI, conjoint, A/B, tracking, etc.), define universo, muestra y cuotas, propone instrumento preliminar, cronograma, presupuesto y proveedor. Selecciona el aliado adecuado (Kantar, Ipsos, YouGov, agencia qualitativa, etc.) considerando costo, tiempo y acceso al público. Usar después de que el brief esté firmado, o cuando el usuario diga "diseñar la metodología", "armar la propuesta metodológica", "qué metodología uso para…", "cómo investigo X".
---

# Skill: Diseño de metodología (Etapa 3 del flujo CI)

## Filosofía aplicada
La metodología debe estar al servicio del **insight**, no del lucimiento técnico. Dimensionar adecuadamente los 3 retos permanentes del equipo: **tiempo, costo y acceso al público**. Una metodología elegante que no se puede ejecutar es fracaso garantizado.

Además, recordar: el aliado **levanta la data**; el equipo **construye el insight**. Elegir aliado técnico bueno pero entender que la interpretación vuelve al equipo.

Leer `Filosofia_Consumer_Insights.md` y `Onboarding_Bancolombia_VP_Mercadeo.md`.

## Propósito
Seleccionar el abordaje metodológico que mejor responda a los objetivos del brief, balanceando rigor, velocidad y presupuesto.

## Cuándo invocar
- Existe un brief firmado y hay que diseñar la ejecución.
- El usuario pregunta por metodología, técnicas, muestra, proveedores.

## Estilo conversacional
Claude debe guiar con preguntas que expongan los trade-offs (*"si tienes 3 semanas y $30M, olvídate de etnografía; ¿qué prefieres sacrificar, profundidad o representatividad?"*), no entregar la propuesta ideal sin discutir restricciones.

## Entradas que debo leer/pedir
1. **Brief firmado** (`BRIEF-*.md`) — obligatorio.
2. **Presupuesto real** (puede diferir del tentativo).
3. **Deadline real** (afecta técnicas viables).
4. Preferencia de proveedor/agencia.

## Pasos que debo ejecutar

1. Leer brief; extraer objetivos específicos y marco dolor/tensión/insight.
2. **Decidir naturaleza del estudio:**

   | Objetivo busca… | Enfoque |
   |---|---|
   | Explorar porqués, descubrir significados, captar emociones y tensión | **Cualitativo** |
   | Medir, dimensionar, cuantificar, comparar, proyectar | **Cuantitativo** |
   | Ambas cosas | **Híbrido** |
   | Seguir KPIs en el tiempo | **Tracking continuo** |

   Regla práctica: para construir **insight** (no solo descripción), el híbrido suele ser el más potente — lo cuali da la tensión y el insight; lo cuanti dimensiona y prioriza.

3. **Seleccionar técnicas específicas:**

   **Cualitativas**
   - IDIs — temas sensibles, decisores B2B (corporativo, gobierno, preferencial), clientes de alto valor.
   - Focus groups — dinámica de grupo, reacción a conceptos.
   - Etnografías / shop-alongs — comportamiento real en sucursal o con la app (Bancolombia, Nequi).
   - Diarios digitales / mobile ethnography — uso cotidiano (Nequi, app Bancolombia, Wompi para merchants).
   - Comunidades online (MROC) — temas extendidos.
   - Co-creación — diseño de producto con clientes.
   - Usability testing — app Bancolombia, Nequi, Sucursal Virtual Personas/Empresas.

   **Cuantitativas**
   - Encuesta online (CAWI) — volumen, costo bajo, sesgo de digitales.
   - CATI — segmentos menos digitales, pensionados, rural.
   - Presencial / en sucursal — poblaciones específicas.
   - In-app survey — clientes actuales en momento de uso.
   - Paneles — tracking estable.
   - Conjoint / MaxDiff — precios, atributos, trade-offs.
   - A/B testing — optimización digital.
   - Segmentación estadística — rediseño de segmentos comerciales.
   - Brand tracking — usar directamente la skill `insights-brand-tracking`.

   **Data secundaria / soporte**
   - Social listening.
   - Data interna (CRM, transaccional, canales).
   - Estudios sindicados (YouGov, Kantar, Ipsos, Merco).

4. **Definir universo y muestra:**
   - Universo: perfil exacto según segmentación oficial Bancolombia.
   - Tamaño muestral: cálculo estadístico (n por error ±3% o ±5%).
   - **Cuotas obligatorias** por segmento, región, edad, género, relación con marca. Para banca de personas distinguir: clientes Bancolombia / clientes Nequi / ambos / solo competencia. Para banca empresarial distinguir: Pyme / Empresas / Corporativo / Gobierno.

5. **Proponer instrumento preliminar** — bloques, no preguntas (preguntas se elaboran en Etapa 4).

6. **Cronograma detallado** con todas las fases.

7. **Presupuesto cerrado** con desglose.

8. **Elección del aliado** — lineamientos:
   - **Kantar** — tracking de marca (relación estratégica del equipo con la marca Bancolombia), estudios cuanti robustos.
   - **Ipsos** — cuanti + quali, pricing, segmentación.
   - **YouGov** — sindicados, velocidad, datos sociodemográficos amplios.
   - **Agencias cualitativas locales** — etnografías, co-creación, reclutamiento especializado.
   - **Paneles propietarios** — opciones ágiles y de menor costo.
   - Criterios: expertise en banca/financiero, capacidad de campo, tiempo de respuesta, calidad de reporte crudo (porque el insight lo construye el equipo).

9. **Checklist legal:** Ley 1581, consentimiento, datos sensibles, validación legal para productos específicos, circulares SFC.

10. **Considerar los 3 retos del equipo:**
    - ¿La metodología es ejecutable en el tiempo disponible?
    - ¿Cabe en el presupuesto real?
    - ¿Tenemos acceso garantizado al público objetivo (especialmente perfiles difíciles: corporativo alto, preferencial, no bancarizados)?

## Entregable

```
PROPUESTA METODOLÓGICA
────────────────────────────────────────────────
Estudio:
Brief asociado:
Fecha:

1. ENFOQUE
   [ ] Cualitativo   [ ] Cuantitativo   [ ] Híbrido
   Justificación (en función de objetivos del brief y del insight que perseguimos):

2. TÉCNICA(S) SELECCIONADA(S)
   Técnica / Justificación / Entregable del aliado

3. UNIVERSO Y MUESTRA
   Universo (segmento de banca + marca del grupo):
   Tamaño muestral: N = ___
   Error estadístico: ± ___%   Confianza: ___%
   Cuotas:

4. INSTRUMENTO PRELIMINAR (bloques)

5. CRONOGRAMA (fase / inicio / fin)

6. PRESUPUESTO (concepto / valor)
   - Campo
   - Incentivos
   - Programación
   - Análisis
   - Honorarios
   - Total

7. ALIADO RECOMENDADO
   Aliado:
   Justificación:
   Qué entrega el aliado:
   Qué construimos nosotros sobre lo del aliado:

8. CHECKLIST LEGAL
   [ ] Habeas data / Ley 1581
   [ ] Consentimiento informado
   [ ] Datos sensibles revisados
   [ ] Revisión SFC si aplica

9. ANÁLISIS DE RETOS DEL EQUIPO
   Tiempo: ejecutable? riesgo?
   Costo: cabe en presupuesto?
   Acceso al público: garantizado?

Aprobación:
Sponsor ________________   Gerente Insights ________________
```

Guardar en `Desktop/Gerencia Consumer Insights/metodologias/MET-YYYY-MM-DD-<titulo>.md`.

## Gate de salida
✅ Metodología aprobada + contrato + habeas data OK + 3 retos evaluados.

## Next step
Invocar `insights-campo`.

## Referencias
- `Anatomia_Insights.md` — para garantizar que la metodología elegida permita levantar Hecho + Motivación + Tensión (no solo hecho).
- `Filosofia_Consumer_Insights.md` — 3 retos permanentes (tiempo, costo, acceso).
- `Flujo_Proceso_Consumer_Insights.md` (Etapa 3).
- `Onboarding_Bancolombia_VP_Mercadeo.md` — segmentos, marcas, competidores.
