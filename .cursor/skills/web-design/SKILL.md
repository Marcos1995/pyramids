---
name: web-design
description: Any page, landing, dashboard or component (HTML/CSS/JSX), or "diseño", "web bonita", "UI", "landing". Google Stitch designs, you integrate.
---

# Web design

Stitch (MCP `stitch`, Gemini) designs; you do not design from scratch.

## Style = `DESIGN.md`

- The repo's `DESIGN.md` holds the style and the Stitch ids. Missing: create it with this default and the user's wishes on top:
  `Minimal y moderno, estilo estudio actual. Mucho aire, jerarquía clara, 1 color de acento, tipografía con carácter. Claro y oscuro. Nada de degradados morados, emojis como iconos, todo centrado ni plantillas genéricas.`
- Existing design (Stitch/Figma export, tokens, components): follow it.

## Steps

1. New page or full restyle: `create_project` once (reuse the project id from `DESIGN.md`), then `generate_screen_from_text` with purpose, real content, the `DESIGN.md` style and `deviceType` (`DESKTOP`; `MOBILE` if mobile-first). Changes to an existing screen: `edit_screens`.
2. `get_screen`: download its HTML and screenshot. Keep layout, palette and type; adapt to the repo stack (static: one HTML + CSS, no build; React: Tailwind v4 + shadcn/ui). No unused CSS/JS, real text.
3. Write the project/screen ids in `DESIGN.md`.
4. Small tweaks (a button, a color, spacing): edit directly, no Stitch.
5. Stitch missing or failing: hand-build following `DESIGN.md`.

## Before HECHO

Responsive 360-1440px without horizontal scroll, WCAG AA contrast, visible focus, `alt` on images, `prefers-reduced-motion`. Look at it with skill `verify`.
