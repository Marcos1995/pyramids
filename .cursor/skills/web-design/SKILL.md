---
name: web-design
description: Modern, minimal, beautiful web UI. Use whenever creating or restyling any page, landing, dashboard or component (HTML/CSS/JSX), or when asked for "diseño", "web bonita", "UI", "landing".
---

# Web design

Goal: looks like a current product from a good studio: minimal, confident, polished. Never a generic "AI template".

## 1. Direction first

- Before code, state in 1 line: purpose, audience, one aesthetic direction (editorial minimal, Swiss grid, soft tech, warm neutral...) and one memorable detail. Commit to it.
- If the repo already has a design source (Google Stitch or Figma export, `DESIGN.md`, existing tokens/components), follow it instead of inventing.

## 2. Stack (match the repo, add nothing unneeded)

- Static / `index.html`: one HTML + modern CSS, no framework, no build. Max 2 font families (Google Fonts / Fontsource, `display=swap`). Icons: inline SVG (Lucide).
- React / Next / Vite: Tailwind v4 + shadcn/ui + `lucide-react`. Motion via CSS; `motion` lib only if CSS can't.
- 3D: not by default. Only for visual/spatial products or when asked: one lazy-loaded hero (Spline embed or three.js) with static fallback.

## 3. System

- Tokens as CSS vars in `:root`: colors in `oklch()`, `color-scheme: light dark` + `light-dark()`, one neutral scale + one accent.
- Type: distinctive display font + clean text font (not Inter/Roboto/Arial alone). Fluid sizes with `clamp()`, headings tight (`letter-spacing: -0.02em`), body 16-18px, `line-height` 1.5-1.6, max 70ch.
- Layout: CSS grid, container queries, `width: min(100% - 2rem, 72rem)`. 4/8px spacing scale, generous whitespace, clear hierarchy.
- Surfaces: 1px low-contrast borders over heavy shadows, one consistent radius. At most one effect (grain, soft gradient, glass), used sparingly.
- Motion: 150-300ms ease-out, subtle reveals (scroll-driven animations, View Transitions). Always honor `prefers-reduced-motion`.

## 4. Avoid

Purple-to-blue gradients on white, emoji as icons, everything centered, identical 3-card grids, "Welcome to X" heroes, lorem ipsum, shadows everywhere, more than one accent color.

## 5. Quality bar (before HECHO)

- Responsive 360px to 1440px, no horizontal scroll.
- WCAG AA contrast, visible `:focus-visible`, semantic HTML, `alt` on images.
- Real hover/active/empty/loading states on interactive parts.
- Fast: no unused libs, images with `width`/`height` + `loading="lazy"`.
- Look at it: skill `verify` (screenshots mobile/desktop, light/dark).
