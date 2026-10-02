# Graph-Greener

Graph-Greener is a Python tool that paints your GitHub contribution graph green by generating backdated commits over a chosen date range. It creates empty commits on the specified branch with custom timestamps, letting you shape your contribution history for demo purposes.

## Features

- Generates backdated commits across any date range you specify
- Random or fixed commit counts per day for a natural-looking graph
- Works with any local Git repository connected to a GitHub remote
- Zero dependencies — pure Python 3 stdlib + the Git CLI
- Interactive CLI prompts (branch, start/end date, commits per day)

## Tech Stack

- Python 3 (stdlib only — `datetime`, `random`, `subprocess`, `os`)

## Quick Start

```bash
cd Graph-Greener-main
python main.py
```

Follow the prompts: target branch, start date, end date, and commits per day. Then push:

```bash
git push origin <branch>
```

Requires Git configured locally and a GitHub repo remote to push the generated commits.

## Project Structure

```
Graph-Greener-main/
├── main.py    # contribution-graph painter script
└── README.md
```

## Environment Variables

None.

## Deploy Notes

This is a command-line tool, not a web app — there is nothing to deploy. Run it locally on your machine.

## Disclaimer

Demo / fun project. Use responsibly — avoid creating fake contribution history on repos where it could be misleading.

## License

Check upstream terms.

---

Built by Girish Lade — https://ladestack.in
