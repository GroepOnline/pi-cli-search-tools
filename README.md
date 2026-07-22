# pi-cli-search-tools

CLI search & filter tools skill voor [Pi.dev](https://pi.dev) — de power-user toolkit voor ripgrep, fzf, jq, awk, sed, grep, find en pipe compositions.

## Wat is dit?

Een Pi skill die de agent leert om **niet-interactive** zoek- en filtercommando's te gebruiken:

- **ripgrep (rg)**: Snelle tekst-zoek met `--json` output voor pipe-verwerking
- **fzf**: Fuzzy finder in non-interactive mode (`--filter`, `--query`)
- **jq**: JSON query-taal voor gestructureerde data
- **awk/sed/grep**: Klassieke Unix text-processing
- **Pipe compositions**: Samengestelde pipelines voor log-analyse, code-exploratie, data wrangling

## Installatie

```bash
# Kloon deze repo naar je Pi skills directory
git clone git@github.com:OnlineChefGroep/pi-cli-search-tools.git ~/.agents/skills/cli-search-tools
```

Of voeg toe aan je Pi settings:

```json
{
  "skills": ["~/.agents/skills/cli-search-tools"]
}
```

## Scripts

- `scripts/search-pi-logs.sh` — Doorzoek Pi sessie-logs (JSONL) met filters

## Gebruik

De skill wordt automatisch geladen door Pi wanneer een taak past bij search/filter/analyse.

```bash
/skill:cli-search-tools
```

## Licentie

Private — ChefGroep fleet only.
