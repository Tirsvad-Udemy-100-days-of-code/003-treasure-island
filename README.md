# 🚀 Treasure Island

A beginner-friendly Python "Choose Your Own Adventure" text game where your choices decide whether you find the treasure.

## 📚 Table of Contents

- [Overview](#-overview)
- [Requirements](#-requirements)
- [Setup](#-setup)
- [Run](#-run)
- [Tests](#-tests)
- [License](#-license)
- [Links](#-links)
- [Appendix: Project documents](#-appendix-project-documents)

## 🧭 Overview

You start at a crossroad and pick your way through the story using `if` / `elif` / `else` logic. Answers are lowercased and trimmed, so `Left` and ` LEFT ` work too, and invalid answers are asked again.

```text
crossroad: left or right
  right -> Game Over (hole)
  left  -> lake: wait or swim
            swim -> Game Over (trout)
            wait -> island: red, yellow or blue door
                      red    -> Game Over (fire)
                      blue   -> Game Over (beasts)
                      yellow -> You Win!
```

Only one path wins. Feel free to rewrite the story in `src/treasure_island/game.py`. It is part of Udemy's *100 Days of Code: The Complete Python Pro Bootcamp* and has no runtime dependencies.

The repository holds the game in `src/treasure_island/`, its tests in `tests/`, the project documents and the [wiki][wiki] pages in `docs/`, and the SQA and QC framework in `framework/`.

## 📋 Requirements

- Python 3.13 or newer
- `pytest` (only for running the tests)

## 🛠️ Setup

Create and activate a local virtual environment in the project root:

```bash
python -m venv .venv
```

Activate it:

- Windows (PowerShell): `.venv\Scripts\Activate.ps1`
- Windows (cmd): `.venv\Scripts\activate.bat`
- Git Bash on Windows: `source .venv/Scripts/activate`
- macOS / Linux: `source .venv/bin/activate`

Install the project with the test tools:

```bash
pip install -e ".[dev]"
```

Leave the environment with `deactivate`.

Optional: copy `.env.example` to `.env` and fill in the tokens you need. They are only used for repository maintenance, never to run the game. `.env` is git-ignored.

## ▶️ Run

```bash
python -m treasure_island
```

or, after installing:

```bash
treasure-island
```

## 🧪 Tests

```bash
pytest
```

## 📄 License

Released under the [GNU Affero General Public License v3.0](LICENSE) (AGPL-3.0-or-later).

## 🔗 Links

- [Repository][repository]
- [Documentation][documentation]
- [Issue tracker][issues]

## 📎 Appendix: Project documents

The documents a newcomer needs, in reading order.

| Document | What it tells you |
| --- | --- |
| [AGENTS.md][agents] | The rules AI agents follow in this repository |
| [Wiki][wiki] | How to play, install and develop the game |
| [Artifact registry][registry] | Where each artifact type lives, the next version, the PO language and domain |
| [Framework README][framework-readme] | The framework this project uses |
| [Framework changelog][framework-changelog] | What changed in each framework release |

---

[repository]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/003-treasure-island
[documentation]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/003-treasure-island/wiki
[issues]: https://git.tirsystem.com/Tirsvad-Udemy-100-days-of-code/003-treasure-island/issues
[agents]: ./AGENTS.md
[wiki]: ./docs/wiki/Home.md
[registry]: ./docs/artifact-registry.md
[framework-readme]: ./framework/README.md
[framework-changelog]: ./framework/CHANGELOG.md
