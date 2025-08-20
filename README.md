# Digitive Website

Sito web per Digitive Business Advisors con strategie digitali, AI e comunicazione per PMI.

## 🚀 Open Graph & Social Media

### Test Validatori

Per testare gli Open Graph:

1. **Facebook Sharing Debugger**
   - https://developers.facebook.com/tools/debug/
   - Incolla URL → "Esegui lo scraping" 2 volte

2. **X/Twitter Card Validator**
   - https://cards-dev.twitter.com/validator
   - Valida l'URL per vedere l'anteprima

3. **LinkedIn Post Inspector**
   - https://www.linkedin.com/post-inspector/
   - Testa come appare su LinkedIn

### Aggiornamento Immagini OG

Per aggiornare le immagini Open Graph:

#### Homepage:
1. Sostituisci `img/og-home-v2.jpg` con la nuova immagine
2. Cambia il nome del file (es. `og-home-v3.jpg`)
3. Aggiorna i meta tags con il nuovo nome

#### Articoli Blog:
1. Crea immagine in `static/img/og/` con formato: `{slug}-{YYYYMMDD}.jpg`
2. Esempio: `intelligenza-artificiale-pmi-20250820.jpg`
3. I social prenderanno automaticamente la nuova immagine

#### Cache Control:
- HTML: `no-cache` (sempre aggiornato)
- Immagini: `immutable` (cache permanente)
- Cambia nome file per forzare aggiornamento

### Specifiche Immagini

- **Dimensioni**: 1200×630px
- **Formato**: JPG o PNG
- **Peso**: < 2MB
- **Homepage**: `img/og-home-v2.jpg`
- **Articoli**: `static/img/og/{slug}-{YYYYMMDD}.jpg`

### Struttura Immagini OG

```
img/
├── og-home-v2.jpg                    # Homepage
└── ...
static/img/og/
├── intelligenza-artificiale-pmi-20250820.jpg
├── minimalismo-digitale-comunicazione-20250820.jpg
└── ...
```

### Host Canonico

- **URL principale**: https://www.digitive.it/
- **Canonical**: Impostato su tutte le pagine
- **Redirect**: Configurare 301 da digitive.it a www.digitive.it

## 📁 Struttura

```
digitive_site/
├── index.html              # Homepage
├── projects.html           # Pagina progetti
├── privacy.html            # Privacy policy
├── blog/
│   ├── index.html          # Lista articoli
│   ├── intelligenza-artificiale-pmi.html
│   └── minimalismo-digitale-comunicazione.html
├── css/
│   └── style.css
├── img/
│   ├── og-digitive.jpg     # Immagine OG principale
│   └── ...
├── static/
│   ├── lottie/            # Animazioni JSON
│   └── img/
│       └── projects/      # Immagini progetti
├── data/
│   └── links.json         # Link curati
├── robots.txt
└── sitemap.xml
```

## 🎨 Features

- **Responsive Design**: Mobile-first
- **Lottie Animations**: Icone animate
- **Modal Projects**: Overlay con dettagli
- **Blog SEO**: Articoli ottimizzati
- **Accessibilità**: WCAG compliant
- **Performance**: Lazy loading, ottimizzazioni

## 🔧 Sviluppo

```bash
# Server locale
python3 -m http.server 8000

# Apri browser
open http://localhost:8000
```
