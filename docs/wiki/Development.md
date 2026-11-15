# Development

🌐 **English**

## Where the code is

| File | Purpose |
| --- | --- |
| `src/treasure_island/game.py` | The story: `play`, the `choose` helper and the `BANNER` |
| `src/treasure_island/__main__.py` | Lets `python -m treasure_island` start the game |
| `tests/test_game.py` | One test per ending, plus input handling |

## Design

The story logic does not read the keyboard or write to the screen itself. Both
are passed in:

- `play(ask=input, say=print)` returns `True` when the player wins and `False`
  otherwise.
- `choose(ask, prompt, options)` asks until the answer, lowercased and trimmed,
  is one of the options.

The game uses the real `input` and `print`; a test passes a function that
returns scripted answers and a list that collects the output, so no test needs
a terminal.

## Change the story

Edit `play` in `src/treasure_island/game.py`. Keep the story in
[How to Play](How-to-Play) in step with the code, and add or change a test for
each ending you add or change.

## Run the tests

```bash
pytest
```

The pytest settings (`testpaths`, `pythonpath`) are in `pyproject.toml`.

## Project documents and the framework

The project follows the SQA and QC framework in `framework/`; the rules the AI
agent follows are in `AGENTS.md`. This wiki is the folder `docs/wiki/`, flat,
as `framework/process/wiki.md` requires, and is published to the git host's
wiki when a change to it is merged to the default branch.
