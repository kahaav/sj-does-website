# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A single-file static website for **SJ DOES** (Suzanne Jeffers, sjdoes.com) — a legal services consultancy offering strategy, marketing, social media, legal tech, recruitment, and coaching. Deployed via GitHub Pages.

## Structure

Everything lives in `index.html`: all HTML, CSS (in a `<style>` block), and no JavaScript. There is no build step, no package manager, and no framework. Editing `index.html` is a direct change to the live site once pushed to `main`.

The CNAME file points GitHub Pages to `sjdoes.com`.

## Design system

CSS custom properties defined in `:root`:

```
--peach: #F4A888        (brand accent, CTAs, headings)
--peach-soft: #FFDCCB   (shop section background)
--peach-light: #FFF5EF  (hover states)
--cream: #F6F1EB        (hero, clients, footer)
--sand: #E8DED2         (borders, grid lines)
--taupe: #CFC2B4
--cocoa: #3B2F2A        (body text, dark elements)
--black: #111111
--white: #FFFFFF
```

Fonts (Google Fonts):
- **Cormorant Garamond** — display/headings, logo, large type
- **Inter** — body copy, navigation, tags, small text

## Page sections (in order)

`#hero` → `#services` → `#hook` (peach strip) → `#clients` → `#values` → `#testimonials` → `#about` → `#shop` → `#contact` → `footer`

Navigation links map directly to these section IDs.

## Deployment

Push to `main` → GitHub Pages rebuilds automatically. No CI, no preview environments.

## Tone and brand voice

The brand voice is warm, direct, and a little cheeky. Key phrase: *"Do you know anyone who does that? SJ Does."* Copy should feel human — not corporate, not generic. The peach emoji (🍑) is a deliberate brand element used throughout.
