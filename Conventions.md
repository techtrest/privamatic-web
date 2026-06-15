# Privamatic Web — Conventions

## Purpose
Landing page for Privamatic, an Android privacy auditing app.
Single HTML file. Deployed via Netlify from this repo.

## Core Rule
One file: `index.html`. Everything inlined. No build step. No framework.

## Brand

### Colours
- Primary: `#004225` (British Racing Green)
- Background: `#FFFBFE`
- Surface/cards: `#F5F5F5`
- Accent/cream: `#FFFDD0`
- Never hardcode any other colours.

### Typography
- System font stack only: `-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`
- Never import external fonts. No Google Fonts. No CDN font links.
- PRIVAmatic typographic treatment: PRIV in bold, matic in regular weight. Always.

### Logo/Name
- Written as PRIVAmatic — not Privamatic, not PRIVAMATIC
- HTML: `<strong>PRIVA</strong>matic`

## Technical Rules

### Dependencies
- Zero external dependencies.
- No CDN links of any kind.
- No third-party scripts.
- No analytics, no tracking pixels, no cookies.
- Images embedded as base64 if needed.

### CSS
- All styles in a single `<style>` block in `<head>`.
- No inline `style=` attributes unless absolutely unavoidable.
- No CSS frameworks (no Tailwind, no Bootstrap).
- Light mode only. No dark mode. No `prefers-color-scheme` switching.

### JavaScript
- Minimal vanilla JS only — Intersection Observer for scroll animations is acceptable.
- No animation libraries (no GSAP, no anime.js, no Motion).
- All animations via CSS. JS only for triggering CSS classes.
- Always include `prefers-reduced-motion` fallback.

### HTML
- Semantic structure: `<header>`, `<main>`, `<section>`, `<footer>`
- Alt text on every image.
- All links open in same tab unless linking to external install pages.

### Animations
- Subtle and purposeful. Nothing loops. Nothing is flashy.
- Score circle draws on scroll into view.
- Sections fade in on scroll.

## Page Structure
1. Hero — tagline, screenshot, F-Droid + GitHub CTAs
2. What it does — three concrete checks
3. Score showcase — animated score circle
4. How to install — F-Droid only, three steps
5. Trust signals — four items, understated
6. Footer — GitHub, F-Droid links, "No cookies. No tracking. No nonsense."

## Copy Voice
- Direct. No marketing fluff. No SaaS clichés.
- Short sentences. Fragments acceptable.
- No exclamation marks in CTAs.
- Specific and honest.
- No filler phrases.

## Links
- F-Droid app page: `https://f-droid.org/packages/com.techtrest.privamatic`
- F-Droid homepage: `https://f-droid.org`
- GitHub: `https://github.com/techtrest/privamatic`

## What NOT to do
- No Google Fonts or any external font service
- No analytics scripts (no Google Analytics, Plausible, Fathom, etc.)
- No dark mode variant
- No JavaScript animation libraries
- No CSS frameworks
- No multiple HTML files — everything in `index.html`
- No lorem ipsum or placeholder content
- No emoji in UI
- Never write "PRIVAmatic" as "Privamatic" or "PRIVAMATIC"

## Before every Claude Code session
Read this file first. Apply all rules to every edit.
