# Paper Search

A Claude Code plugin and skill for searching academic papers via [OpenAlex](https://openalex.org/) (250M+ works, free, no API key).

## Plugin Install

```bash
claude plugin marketplace add ykdojo/paper-search
claude plugin install paper-search@paper-search
```

## Scripts

Scripts are in the `scripts/` directory:

- **`scripts/search.sh`** — keyword search with relevance/cites/date sorting and pagination
- **`scripts/paper.sh`** — detailed lookup by DOI or OpenAlex ID

## Skills

- **`paper-search`** — see `skills/paper-search/SKILL.md` for full instructions
