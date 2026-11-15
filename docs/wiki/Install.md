# Install

🌐 **English**

## Requirements

- Python 3.13 or newer
- `pytest`, only to run the tests

## Set up

Create a virtual environment in the project root:

```bash
python -m venv .venv
```

Activate it:

- Windows (PowerShell): `.venv\Scripts\Activate.ps1`
- Windows (cmd): `.venv\Scripts\activate.bat`
- Git Bash on Windows: `source .venv/Scripts/activate`
- Linux and macOS: `source .venv/bin/activate`

Install the game, with the development dependencies:

```bash
pip install -e ".[dev]"
```

## Run

```bash
treasure-island
```

or, without the command:

```bash
python -m treasure_island
```

## Check that it works

```bash
pytest
```

All tests pass when every path of the story behaves as described in
[How to Play](How-to-Play).
