# paper-search

A Claude Code plugin and skill for searching academic papers via the [OpenAlex API](https://docs.openalex.org/).

## Install as Claude Code Plugin

```bash
claude plugin marketplace add delfinadap/paper-search
claude plugin install paper-search@paper-search
```

After installing, the `paper-search` skill is available automatically. Just ask Claude Code to search for papers and it will use the skill.

## Requirements

- `curl`, `jq`

## Usage

```bash
# Search for papers (sorted by relevance by default)
scripts/search.sh "mindfulness meditation stress reduction" 10

# Sort by citation count
scripts/search.sh "mindfulness meditation stress reduction" 10 cites

# Sort by publication date
scripts/search.sh "mindfulness meditation stress reduction" 10 date

# Page 2 of results
scripts/search.sh "mindfulness meditation stress reduction" 10 relevance 2

# Get 25 results per page
scripts/search.sh "mindfulness meditation stress reduction" 25

# Look up a specific paper by DOI
scripts/paper.sh "https://doi.org/10.1073/pnas.0407162101"

# Look up by OpenAlex ID
scripts/paper.sh W2097529540
```

## API

Uses [OpenAlex](https://openalex.org/) — free, open, no API key required. 250M+ works indexed.

Initially introduced in [45 Claude Code Tips](https://github.com/ykdojo/claude-code-tips) (Tip 27).

