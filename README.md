# tokenpurse

Estimate LLM cost of a file before you send it

Built for my own use; public in case it helps someone.

## Installation

```bash
# stdlib only
```

## Features

- Heuristic token estimate (~4 chars/token)
- Reports input/output tokens and USD estimate
- Zero dependencies
- Per-model pricing table in JSON

## Examples

```bash
python cost.py prompt.txt --model gpt-4o-mini --expect-out 500
```

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── pull_request_template.md
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── cost.py
└── pricing.json
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## FAQ

**Is this production ready?**  
It works for my use case; review the code before relying on it.

**Why no framework?**  
The stdlib covers what this project needs.
