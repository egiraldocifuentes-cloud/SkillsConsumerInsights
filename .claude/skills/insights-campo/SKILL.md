---
name: insights-campo
description: Prepara, ejecuta y monitorea el campo de una investigación — redacta el cuestionario o guía, diseña el piloto, define controles de calidad, monitorea avance de muestra y cuotas, aplica quality checks y produce el reporte de campo final. Mantiene la relación con el aliado asegurando que la data llegue apta para que el equipo la interprete. Usar después de que la metodología esté aprobada, o cuando el usuario diga "armar el cuestionario", "diseñar la guía", "preparar el piloto", "salir a campo", "monitorear el campo", "reporte de campo".
---

# Skill: Ejecución de campo (Etapa 4 del flujo CI)

## Filosofía aplicada
El aliado ejecuta el campo; **el equipo supervisa la calidad** de ese campo para asegurarse de que la data que llega permite construir insight. Un campo mal hecho obliga a escribir un informe mensajero (solo describe lo que el aliado entregó). Aquí se protege la materia prima del insight.

Además: el instrumento (cuestionario o guía) es donde empieza a construirse el insight — cada pregunta debe nacer del marco dolor/tensión/insight definido en el brief, no de curiosidad abierta.

Leer `Filosofia_Consumer_Insights.md` y `Onboarding_Bancolombia_VP_Mercadeo.md`.

## Propósito
Levantar información con calidad, rigor metodológico y cumplimiento legal, asegurando que la data que reciba el equipo sea interpretable.

## Cuándo invocar
- Metodología aprobada y hay que diseñar el instrumento.
- Campo en curso que hay que monitorear.
- Cierre de campo y reporte final.

## Entradas
1. **Propuesta metodológica** (`MET-*.md`).
2. **Brief original** — para no perder foco.
3. Conceptos/atributos/precios/prototipos a testear si aplica.

## Pasos

### 4.1. Diseño del instrumento

**Cuantitativo:**
1. Traducir cada objetivo específico y cada elemento del marco dolor/tensión/insight a preguntas concretas.
2. Bloques típicos:
   - Screening y filtros.
   - Contexto y hábitos.
   - Conocimiento y consideración de marca (para Bancolombia y competidores: Grupo Aval, Grupo Bolívar, neobancos).
   - Uso y recordación.
   - Atributos / imagen de marca.
   - Experiencia del cliente (CX omnicanal, NPS, CSAT — considerar impacto de eventos como caídas masivas).
   - Testeo de concepto / precio / producto si aplica.
   - Clasificación sociodemográfica y de banca.
3. Lógica de salto, filtros, cuotas.
4. Alternancia de escalas, evitar sesgos de orden.
5. Lenguaje neutral — sin sugerencia, doble negación, asunciones.
6. **Checklist de calidad:**
   - [ ] Cada pregunta responde a un objetivo del brief (no hay huérfanas).
   - [ ] Las preguntas clave atacan tensión/insight, no solo dolor.
   - [ ] Longitud < 15–18 min (drop-out).
   - [ ] Lenguaje claro para el segmento.
   - [ ] Escalas consistentes (no mezclar 1–5 con 0–10 sin razón).
   - [ ] Habeas data y consentimiento al inicio.
   - [ ] Preguntas sobre productos específicos revisadas por legal.
   - [ ] Cuando el estudio es de la propia marca → blind study (encubrir sponsor).

**Cualitativo (guía de moderación):**
- Bienvenida y consentimiento.
- Calentamiento.
- Preguntas abiertas por bloque (exploración → tensión → reacción a estímulos).
- Dinámicas proyectivas (laddering, asociación libre, storytelling, trade-offs).
- Cierre.
- Siempre incluir al menos un bloque diseñado para provocar la **articulación de tensión** por parte del participante.

### 4.2. Piloto
1. Tamaño: 5–15% de muestra cuanti; 1–2 sesiones quali.
2. Objetivos: detectar preguntas mal formuladas, medir tiempo real, validar programación, probar reclutamiento.
3. Ajustes antes de salida formal.

### 4.3. Salida a campo
1. Programación en plataforma.
2. Iniciar reclutamiento.
3. **Monitoreo diario:**
   - Avance vs. cuotas.
   - Tasa de respuesta y completitud.
   - Quality checks automáticos: straight-lining, tiempos mínimos, duplicados, IPs repetidas, inconsistencias entre bloques.

### 4.4. Controles de calidad
- Validación de identidad y perfil.
- Supervisión 10–20% del campo (CATI, presencial).
- Limpieza de respuestas sospechosas.

### 4.5. Cierre de campo
1. Verificar cuotas y balance muestral.
2. **Base de datos depurada** (cuanti) en SPSS/CSV/Excel con diccionario de variables.
3. **Transcripciones + audiovisual** (quali) con consentimientos.
4. **Reporte de campo**.

## Entregables

1. **Cuestionario o guía final** (markdown).
2. **Plan de piloto** — muestra, objetivos, criterios de ajuste.
3. **Plan de monitoreo** (dashboard o tabla de avance).
4. **Reporte de campo:**

```
REPORTE DE CAMPO
────────────────────────────────────────────────
Estudio:
Aliado:
Fechas de campo:
Universo:
Muestra lograda: N = ___ (vs. meta: ___)
Cumplimiento de cuotas (por segmento y marca):
Tasa de respuesta: ___%
Tasa de completitud: ___%
Incidencias:
Quality checks aplicados:
Entregables: [base, transcripciones, audios]

FILTRO DE FILOSOFÍA (pre-análisis)
[ ] La data permite construir insight, no solo describir
[ ] Hay suficiente evidencia de tensión (no solo dolor manifiesto)
[ ] Cuotas permiten cortes para el bisturí que persigue el brief
```

Guardar en `Desktop/Gerencia Consumer Insights/campo/<codigo-estudio>/`.

## Gate de salida
✅ Base/transcripciones entregadas + reporte aprobado + cuotas cumplidas + filtro de filosofía OK.

## Buenas prácticas críticas
- **Nunca** ir a campo sin piloto.
- **Blind study** cuando la marca estudiada es del grupo.
- Validación legal previa para preguntas sobre productos específicos.
- Ley 1581 en cada contacto.

## Next step
Invocar `insights-analisis`.

## Referencias
- `Anatomia_Insights.md` — las preguntas del instrumento deben permitir capturar Hecho, Motivación y Tensión (no solo Hecho).
- `Filosofia_Consumer_Insights.md`.
- `Flujo_Proceso_Consumer_Insights.md` (Etapa 4).
- `Onboarding_Bancolombia_VP_Mercadeo.md` — cuotas por segmento, marcas, competidores.
