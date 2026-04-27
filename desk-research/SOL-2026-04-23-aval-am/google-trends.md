# Señales de interés digital — Google Trends (T6, ESBOZO)
## Fase 1 — Escucha competitiva

**Estado:** ESBOZO por alcance acordado con Juango (nivel b). La ejecución técnica completa requiere apertura directa de trends.google.com — Google Trends no expone consistentemente series históricas vía fetch programático.

**Recomendación operativa:** que el analista humano corra manualmente los términos de abajo el viernes 24 AM y pegue screenshots de series temporales en este archivo. Tiempo estimado: 30 minutos.

---

## Términos a consultar (catálogo listo)

### Familia Aval
1. `"Aval Fiduciaria"` (término exacto)
2. `"Meta Decidida"` (término exacto)
3. `"Aval Asset Management"` (término exacto)
4. `BlackRock Colombia` (libre)

### Familia Cibest / Bancolombia
5. `"Cibest Capital"` (término exacto)
6. `"Valores Bancolombia"` (término exacto)
7. `"Fiduciaria Bancolombia"` (término exacto)

### Categoría (contexto de mercado)
8. `fondos de inversión` (Colombia)
9. `asset management` (Colombia)
10. `inversión internacional` (Colombia)

---

## Ventanas temporales

| Ventana | Propósito |
|---|---|
| **12 meses** (23-abr-2025 → 23-abr-2026) | Baseline histórico. Detectar si Cibest Capital, Valores Bancolombia y Fiduciaria Bancolombia tenían alguna estacionalidad antes del hito Aval. Detectar pico por consolidación Aval (ene-2026). |
| **90 días** (23-ene-2026 → 23-abr-2026) | Foco período del estudio. Detectar picos por consolidación Aval (ene-2026), entrevistas pre-lanzamiento (abr), lanzamiento Meta Decidida (21-abr). |
| **7 días** (17-abr → 23-abr-2026) | Densidad post-lanzamiento. Validar si el pico del 21-abr está durando o ya bajó. |

---

## Geografía

- Colombia (nacional) — baseline principal.
- Desglose por regiones principales si el volumen lo permite: Bogotá, Medellín, Cali, Barranquilla.
- Regiones con mayor concentración de alto patrimonio: Bogotá + Medellín (prioridad).

---

## Hipótesis previas a la consulta (para validar con la data real)

| # | Hipótesis | Razón |
|---|---|---|
| H1 | Pico claro de búsquedas *"Meta Decidida"* el 21-22 de abril | Cobertura coordinada de prensa ese día |
| H2 | Pico anterior de *"Aval Fiduciaria"* el 1-5 enero (consolidación) | Cobertura de Semana, Valora, El Tiempo en esa ventana |
| H3 | Baseline muy bajo (~0) de *"Cibest Capital"* en Colombia | Cibest Capital posicionado a audiencia US; en Colombia el término es interno |
| H4 | Pico pequeño de *"Valores Bancolombia"* el 10-nov-2025 (lanzamiento Marketplace) | Cobertura de Valora, La República, Noticias Caracol |
| H5 | Tendencia estable de *"fondos de inversión"* sin picos específicos | Categoría madura, interés constante |
| H6 | *"BlackRock Colombia"* con pico post 21-abr | Amplificación del partner + su propia narrativa local |

---

## Resultados (a llenar por analista humano)

*(pegar screenshots + breve lectura por término)*

### Aval vs Cibest — serie 90 días
*(pendiente captura)*

### Aval vs Cibest — serie 12 meses (baseline)
*(pendiente captura)*

### Pico post-Meta Decidida (7 días)
*(pendiente captura)*

---

## Observaciones esperables (para confirmar o desmentir tras captura)

Si las hipótesis H1, H3 y H6 se confirman, el hallazgo clave es:
> **Aval logró generar un pico de atención digital sobre *un producto específico* (Meta Decidida) + sobre *la categoría* (asset management / inversión internacional), mientras que el nombre "Cibest Capital" es aún invisible para el buscador colombiano.**

Esto no cambia el diagnóstico central de asimetría narrativa pero aporta un **proxy cuantitativo de atención pública** que permite al sponsor dimensionar el impacto sin depender solo de cobertura mediática.

---

## Limitación declarada al informe

El desk research de Fase 1 entrega Google Trends en modo esbozo. Las series temporales reales se pueden incorporar al informe del lunes si el analista humano ejecuta la consulta el viernes; si no, se declara como limitación y se propone capturarlas en la próxima ola de monitoreo ongoing.
