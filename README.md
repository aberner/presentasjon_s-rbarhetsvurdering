# Hvordan angripe kjente sårbarheter i din applikasjon?

Presentasjon om sårbarhetsvurdering av tredjepartsbiblioteker

**Live presentasjon:** https://aberner.github.io/presentasjon_s-rbarhetsvurdering

## Om presentasjonen

Reveal.js-presentasjon som fokuserer på hvordan man kan identifisere og håndtere kjente sårbarheter i tredjepartsbiblioteker. Bruker Reveal.js 5.2.1 fra CDN for enkelt oppsett uten byggesteg.

## Kjøre lokalt

Presentasjonen krever en HTTP-server på grunn av ES modules. Velg en metode:

### NPM (Anbefalt)

```bash
npm install
npm start
```

Åpne http://localhost:8000

### Python

```bash
python -m http.server 8000
```

Åpne http://localhost:8000

### VS Code Live Server

Høyreklikk på `index.html` → "Open with Live Server"

## Redigere presentasjonen

Rediger `index.html` og oppdater nettleseren for å se endringene. Innholdet ligger mellom `<div class="slides">` taggene.

**Dokumentasjon:** [revealjs.com](https://revealjs.com/)

## Filstruktur

```txt
├── index.html          # Hovedpresentasjonsfil
├── css/               # Stilark for Reveal.js og temaer
├── js/                # Reveal.js JavaScript-filer
├── lib/               # Biblioteker (syntax highlighting, etc.)
├──Deployment

Pushes til `main`-branchen publiseres automatisk på GitHub Pages.

## Teknisk informasjon

- **Framework:** Reveal.js 5.2.1 (CDN)
- **Ingen byggesteg:** Statiske filer klare til bruk
- **Dev server:** http-server (kun for lokal utvikling)
