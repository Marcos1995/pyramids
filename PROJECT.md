<!-- managed-by-telegram-cursor-bot:agent-kit -->
# Contexto del proyecto

## Produccion
- URL: https://github.com/Marcos1995/pyramids
- Vista: https://Marcos1995.github.io/pyramids/ (repo público; Chrome)
- Vista local: `index.html`

## Estado
- Página estática en español: afirmaciones de Biondi (Keops retractado, Kefrén sin revisar, esfinge de 2026 sin artículo), animaciones esquemáticas y la datación/obra según la arqueología.
- La sección «Novedades científicas» es donde se añaden hechos nuevos, del más reciente al más antiguo, cada uno con fuente y estado (revisado, no revisado, retractado o contradicho).
- Las figuras son esquemas propios. No hay datos COSMO-SkyMed ni una réplica del procesado.

## Stack
- HTML, CSS y JS en un solo archivo (`index.html`). Sin build ni dependencias.

## Comandos utiles
- Instalar: nada
- Test: abrir `index.html` en Chrome
- Dev: abrir `index.html`

## Notas para el agente
- No inventar cifras: cada afirmación de la página tiene que poder rastrearse en las fuentes del final.
- No incrustar imágenes de artículos ni de la rueda de prensa.
- Los hechos nuevos van en `index.html`, sección `#novedades`, arriba del todo de esa cronología, con fecha, fuente y estado. No reescribir el resto para «actualizar» un dato.
- Lean kit (ver AGENTS.md)
