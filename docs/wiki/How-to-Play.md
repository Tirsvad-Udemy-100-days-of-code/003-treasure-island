# How to Play

🌐 **English**

You start at a crossroad and answer each question by typing one of the offered
words. Answers are lowercased and trimmed, so `Left` and ` LEFT ` work too, and
an answer that is not one of the options is asked again.

## The story

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

## Endings

| Your choices | Result |
| --- | --- |
| `right` | You fell into a hole. Game Over. |
| `left`, `swim` | You were attacked by angry trout. Game Over. |
| `left`, `wait`, `red` | You were burned by fire. Game Over. |
| `left`, `wait`, `blue` | You were eaten by beasts. Game Over. |
| `left`, `wait`, `yellow` | You found the treasure. You Win! |

Only one path wins. Run the game with the steps on the [Install](Install) page.
