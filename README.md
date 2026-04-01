# Norefjell Trail 22K — Treningsplan

Live: https://norefjell-trail-plan.netlify.app

## Oppdatere planen

1. Last ned ny `plan.json` fra Claude
2. Erstatt filen i denne mappen
3. Push til GitHub:

```bash
git add plan.json
git commit -m "Oppdater treningsplan"
git push
```

Netlify deployer automatisk innen ~30 sekunder.

## Filer

- `index.html` — UI (endres sjelden)
- `plan.json` — Treningsdata (oppdateres av Claude)
- `netlify.toml` — Netlify-konfigurasjon
