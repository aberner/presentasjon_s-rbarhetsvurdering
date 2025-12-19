# Hvordan angripe kjente sårbarheter i din applikasjon?

Presentasjon i sårbarhetsvurdering av tredjepartsbiblioteker

**Live presentasjon:** https://aberner.github.io/presentasjon_s-rbarhetsvurdering

## Om presentasjonen

Denne Reveal.js-presentasjonen fokuserer på hvordan man kan identifisere og håndtere kjente sårbarheter i tredjepartsbiblioteker. Presentasjonen er designet som en innholdsbasert løsning uten behov for byggeverkøy.

## Kjøre presentasjonen lokalt

Du trenger en enkel HTTP-server for å kjøre presentasjonen lokalt. Velg en av metodene nedenfor:

### Metode 1: NPM (Anbefalt for Node.js-brukere)

```bash
npm install
npm start
```

Dette vil installere nødvendige avhengigheter og starte en HTTP-server på port 8000. Åpne deretter http://localhost:8000 i nettleseren.

### Metode 2: Python 3

```bash
python3 -m http.server 8000
```

Åpne http://localhost:8000 i nettleseren.

### Metode 3: Python 2

```bash
python -m SimpleHTTPServer 8000
```

Åpne http://localhost:8000 i nettleseren.

### Metode 4: VS Code Live Server

1. Installer "Live Server"-utvidelsen i VS Code
2. Høyreklikk på `index.html`
3. Velg "Open with Live Server"

### Metode 5: Direkte åpning i nettleser (begrenset funksjonalitet)

Du kan også åpne `index.html` direkte i nettleseren, men noen funksjoner kan være begrenset på grunn av CORS-restriksjoner.

## Redigere presentasjonen

1. Åpne `index.html` i din favoritt teksteditor
2. Rediger innholdet mellom `<div class="slides">` og `</div>`
3. Lagre filen
4. Oppdater nettleseren for å se endringene

### Reveal.js-dokumentasjon

For mer informasjon om hvordan du kan tilpasse presentasjonen, se:
- [Reveal.js på GitHub](https://github.com/hakimel/reveal.js)
- [Reveal.js dokumentasjon](https://revealjs.com/)

## Filstruktur

```
├── index.html          # Hovedpresentasjonsfil
├── css/               # Stilark for Reveal.js og temaer
├── js/                # Reveal.js JavaScript-filer
├── lib/               # Biblioteker (syntax highlighting, etc.)
├── plugin/            # Reveal.js plugins
├── img/               # Presentasjonsbilder og -videoer
└── package.json       # Minimal konfigurasjon for npm start
```

## Deployment til GitHub Pages

Presentasjonen er allerede konfigurert for GitHub Pages. Nye endringer pushet til `main`-branchen vil automatisk bli publisert.

**Merk:** GitHub Pages serverer de statiske filene direkte - ingen HTTP-server eller npm-pakker er nødvendig for produksjonsmiljøet. `http-server` er kun en lokal utviklingsavhengighet.

## Teknisk informasjon

- **Framework:** Reveal.js 3.9.2
- **Ingen byggesteg kreves:** Alle filer er ferdig bygget og klare til bruk
- **Ingen avhengigheter:** Alle nødvendige biblioteker er inkludert i repository

## Lisens

MIT
