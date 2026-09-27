---
name: decide
description: Scored decision for non-trivial choices (stack, library, data model, architecture, scope) or "qué es mejor"/"decide". Logs one line in docs/DECISIONES.md.
---

# Decide

Structured decision, no free-form essay. Uses the current model only: no external API, no extra cost.

## Steps

1. Read `docs/DECISIONES.md` (if present). Reuse a past decision if it still applies; say so.
2. Frame one question. List 2-4 concrete options (always include "lo más simple que funcione").
3. Score each option 1-5 on:
   - **coste** — 0 € extra beyond Cursor Pro = 5; any paid API/subscription = 1
   - **simple** — fewer files, deps and moving parts
   - **encaja** — fits the existing stack and `PROJECT.md`
   - **reversible** — easy to undo or swap later
4. Pick the highest total. Confidence: `alta` (clear winner), `media` (≤2 points gap), `baja` (tie or missing data).
   - `baja` → choose the most reversible option and note what data would change the call.
5. Append one line to `docs/DECISIONES.md` (create it with a `# Decisiones` header if missing):
   `YYYY-MM-DD · <decisión> · <por qué> · descartado: <opciones> · confianza: <alta|media|baja>`
6. Continue the task with the chosen option. Do not ask the user (headless).

## Reply (decision-only requests)

Max 5 lines:

```
DECISIÓN: <opción> (confianza <alta|media|baja>)
Por qué: <1 línea>
Descartado: <opción — motivo>
Siguiente paso: <1 línea>
```
