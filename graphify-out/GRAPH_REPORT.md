# Graph Report - pyramids  (2026-09-27)

## Corpus Check
- 10 files · ~6,498 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 2 file(s) not represented in the graph (top: .mdc 2)

## Summary
- 42 nodes · 32 edges · 10 communities (7 shown, 3 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Debug
- Web design
- Contexto del proyecto
- Verify (UI)
- Agent rules
- Decide
- Review
- README.md

## God Nodes (most connected - your core abstractions)
1. `Debug` - 6 edges
2. `Web design` - 6 edges
3. `Contexto del proyecto` - 6 edges
4. `Verify (UI)` - 4 edges
5. `Decide` - 3 edges
6. `Review` - 3 edges
7. `Agent rules` - 3 edges
8. `1. Root cause` - 1 edges
9. `2. Compare` - 1 edges
10. `3. Hypothesis` - 1 edges

## Surprising Connections (you probably didn't know these)
- None detected - all connections are within the same source files.

## Communities (10 total, 3 thin omitted)

### Community 0 - "Debug"
Cohesion: 0.29
Nodes (6): 1. Root cause, 2. Compare, 3. Hypothesis, 4. Fix, Debug, Red flags → back to step 1

### Community 1 - "Web design"
Cohesion: 0.29
Nodes (6): 1. Direction first, 2. Stack (match the repo, add nothing unneeded), 3. System, 4. Avoid, 5. Quality bar (before HECHO), Web design

### Community 2 - "Contexto del proyecto"
Cohesion: 0.29
Nodes (6): Comandos utiles, Contexto del proyecto, Estado, Notas para el agente, Produccion, Stack

### Community 3 - "Verify (UI)"
Cohesion: 0.40
Nodes (4): 1. Screenshots, 2. Look, 3. Fix and repeat, Verify (UI)

### Community 4 - "Agent rules"
Cohesion: 0.50
Nodes (3): Agent rules, Flujo, Think → Simple → Surgical → Verify (Karpathy)

### Community 5 - "Decide"
Cohesion: 0.50
Nodes (3): Decide, Reply (decision-only requests), Steps

### Community 6 - "Review"
Cohesion: 0.50
Nodes (3): Check, Do, Review

## Knowledge Gaps
- **25 isolated node(s):** `1. Root cause`, `2. Compare`, `3. Hypothesis`, `4. Fix`, `Red flags → back to step 1` (+20 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 35 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **3 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What connects `1. Root cause`, `2. Compare`, `3. Hypothesis` to the rest of the system?**
  _25 weakly-connected nodes found - possible documentation gaps or missing edges._