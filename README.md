# reAIding companion — Landing page

Landing page statica per **reAIding companion**, il compagno di lettura AI senza spoiler di Little Elsewhere.
Un unico file `index.html`: zero build, zero dipendenze. Bilingue IT/EN con toggle, tema chiaro/scuro con override manuale.
Identità: palette Material 3 della PWA (chiaro/scuro automatici), tipografia Charter/Iowan, logo ufficiale inline.

- **App**: https://reaiding-companion.pages.dev/
- **Landing (target)**: https://reaiding-home.pages.dev/

## Deploy su Cloudflare Pages

1. Cloudflare Dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**
2. Seleziona il repository `reAIding-companion-landing` e il branch `main`
3. **Project name**: `reaiding-home` → URL finale `https://reaiding-home.pages.dev`
4. Framework preset: **None** · Build command: (vuoto) · Build output directory: `/`
5. **Save and Deploy**

Da quel momento ogni push su `main` pubblica automaticamente la nuova versione.

## Anteprima locale

Apri `index.html` nel browser. Fine.

## Struttura

```
index.html   ← l'intero sito: CSS, JS e icone SVG inline
icon.svg     ← logo ufficiale della PWA (usato come favicon)
README.md    ← questo file
```

## Dettagli

- **Spoiler Shield progressivo**: le sezioni sono "capitoli" che si sbloccano allo scroll, come la lettura nell'app
- **Tema**: automatico col sistema + toggle manuale (persiste in localStorage)
- **Lingua**: IT/EN con toggle (persiste in localStorage)
- Copia e struttura iterate dal canvas "reAIding companion — Anteprima landing"
