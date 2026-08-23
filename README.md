# pi-cli-search-tools

Power-user search and filtering skill for [Pi](https://pi.dev): ripgrep, fzf, jq, awk, sed, grep, find, xargs, and non-interactive pipe compositions.

## Install with Pi

```bash
pi install npm:@groeponline/pi-cli-search-tools
```

The npm package exposes `SKILL.md` directly through its Pi manifest, so Pi loads the `cli-search-tools` skill automatically.

## What it covers

- **ripgrep (`rg`)**: fast text search, JSON output, file filtering, context and counts
- **fzf**: non-interactive fuzzy filtering with `--filter` and `--query`
- **jq**: structured JSON extraction, filtering and transformations
- **awk / sed / grep / find / xargs**: composable Unix text-processing patterns
- **pipe compositions**: practical recipes for logs, code exploration and data wrangling

## Git install

```bash
git clone https://github.com/GroepOnline/pi-cli-search-tools.git ~/.agents/skills/cli-search-tools
```

Or point Pi at the cloned skill in settings:

```json
{
  "skills": ["~/.agents/skills/cli-search-tools"]
}
```

## Included helper

`scripts/search-pi-logs.sh` searches Pi session JSONL logs with non-interactive filters.

## License

MIT
