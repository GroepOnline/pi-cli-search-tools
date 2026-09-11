<h1 align="center">Pi CLI Search Tools</h1>

<p align="center"><strong>Give Pi better command-line search instincts.</strong><br>Teach agents practical, non-interactive patterns for ripgrep, fzf, jq, awk, sed, grep, find, xargs and pipe-heavy investigation.</p>

<p align="center">
  <a href="https://www.npmjs.com/package/@groeponline/pi-cli-search-tools"><img src="https://img.shields.io/npm/v/@groeponline/pi-cli-search-tools.svg" alt="npm version"></a>
  <a href="https://pi.dev/packages/@groeponline/pi-cli-search-tools"><img src="https://img.shields.io/badge/Pi-package-9b59b6.svg" alt="Pi package"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-green.svg" alt="MIT license"></a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/GroepOnline/pi-cli-search-tools/main/docs/images/cli-search-flow.svg" alt="Pi CLI Search Tools turns a coding question into a deterministic non-interactive shell pipeline" width="100%">
</p>

The skill does not add another search service. It teaches Pi when to use the shell tools already on the machine and how to compose them without interactive dead ends.

## Start in 10 seconds

```bash
pi install npm:@groeponline/pi-cli-search-tools
```

The package exposes `SKILL.md` through its Pi manifest, so the `cli-search-tools` skill loads automatically.

## What changes after install

Instead of reaching for ad-hoc shell pipelines, the agent gets reusable patterns for:

- **ripgrep (`rg`)** — scoped code search, context, counts, file filters and JSON output;
- **fzf** — deterministic non-interactive filtering with `--filter` and `--query`;
- **jq** — extracting, reshaping and filtering structured JSON;
- **awk / sed / grep / find / xargs** — composable text and filesystem investigation;
- **pipe compositions** — logs, repository discovery and lightweight data wrangling.

## Typical use

Ask Pi to use the skill when a task needs broad search or shell-side filtering, for example:

```text
Use cli-search-tools to find every place this config key is read, group matches by package, and show only unique files.
```

Or:

```text
Use cli-search-tools to inspect these JSONL logs and summarize the most common failing tool names.
```

The skill favors non-interactive commands so runs remain reproducible and agent-friendly.

## Install from git

```bash
git clone https://github.com/GroepOnline/pi-cli-search-tools.git ~/.agents/skills/cli-search-tools
```

Or point Pi at the cloned skill:

```json
{
  "skills": ["~/.agents/skills/cli-search-tools"]
}
```

## Included helper

`scripts/search-pi-logs.sh` searches Pi session JSONL logs with non-interactive filters.

## License

MIT © GroepOnline
