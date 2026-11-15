# RabbitHollow Knight 🐇⚔️

Jednostránková pixel-art hra RabbitHollow Knight. Projekt zůstává bez build procesu a externích runtime závislostí.

## Nasazení na Vercel

1. Importuj GitHub repozitář do Vercelu.
2. Framework Preset: **Other**.
3. Root Directory: `./`.
4. Build Command: prázdný / vypnutý.
5. Output Directory: `.`.
6. Install Command: prázdný / vypnutý.

Vercel servíruje `index.html` jako statický web. Hlavičky a bezpečnostní pravidla nastavuje `vercel.json`. Po propojení GitHubu Vercel automaticky vytváří deploymenty při dalších commitech.

## Lokální spuštění

Otevři `index.html` v prohlížeči nebo spusť:

```bash
python -m http.server 8080
```

## Architektura

- Vanilla HTML, CSS a JavaScript.
- Herní canvas běží v prohlížeči.
- Uložení postupu používá úložiště prohlížeče (localStorage).
- Bez serverové databáze, API klíčů, Node runtime nebo build pipeline.
- Základní bezpečnostní HTTP hlavičky a Content Security Policy.

## Omezení

Postup není synchronizovaný mezi zařízeními; zůstává v konkrétním prohlížeči. CSP povoluje inline skripty a styly, protože současná aplikace je single-file HTML. Při budoucím rozdělení assetů lze pravidla dále zpřísnit.
