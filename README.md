# CLS Caribe Legal Services — Website

Bilingual marketing site for **CLS Caribe Legal Services**, a law firm in Costa Rica's Caribbean region. Built and maintained by [VizaCat](https://vizacat.com) — AI Visibility / Answer & Generative Engine Optimization.

**Live:** [cls-legal.vercel.app](https://cls-legal.vercel.app) (preview) · [clslegalcr.com](https://clslegalcr.com) (production — pending cutover)

---

## Stack

- **[Astro](https://astro.build/)** — static site generator
- **Vercel** — hosting + edge delivery
- **Vanilla CSS** — scoped per-component via Astro's `<style>` blocks
- **No JavaScript framework** — minimal client-side JS, optimized for AI crawlers and Lighthouse scores

## Languages

- Spanish (default) — `/`, `/servicios`, `/nosotros`, `/contacto`
- English — `/en/`, `/en/services`, `/en/about`, `/en/contact`

## AI Visibility Features

- Schema.org `LegalService` structured data on every page
- FAQ structured data on homepage
- `llms.txt` for AI crawler briefing
- Open Graph + Twitter card meta for clean link previews
- Bilingual content for expat market capture

## Local Development

```bash
npm install
npm run dev      # local dev server at localhost:4321
npm run build    # build to ./dist
npm run preview  # preview the production build locally
```

## Deployment

Auto-deploys on push to `main` via Vercel. Manual deploy: `vercel --prod`.

## Brand

Per CLS's official brand manual (designed by Rebeca Escalante):

- **Mustard Yellow** `#DEAA09`
- **Charleston Green** `#282C2D`
- **Davy's Grey** `#4E5354`
- **Stormcloud** `#4E6365`
- **Ghost White** `#FAFDFE`
- Typography: **Arial**

---

© CLS Caribe Legal Services. Built by VizaCat.
