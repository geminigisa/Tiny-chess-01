[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/geminigisa/Tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/geminigisa/Tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

# tiny-chess-01 — V3 entry

A compact chess engine in a single Python file (`main.py`, 4,085 bytes).

## Approach

- Late Move Reduction (LMR) with 1 killer move per ply.
- Node budget: 250,000 nodes per move.
- Packed as a single line to fit the 4,096-byte entry limit.

## Trial results

- Trial Elo: **1,530** (16 games: 6 wins, 8 draws, 2 losses).
- Above the 1,450 target and the V0 baseline average of 1,441.

## How to run

Run the engine with:

```
python3 main.py
```

## Local grading

`makefun grade-local` could not run this Python entry on this machine: the process sandbox runs node22 only, and python3.13 runs only inside Docker (`sandbox: the process sandbox runs node22 only (python3.13 runs only inside Docker)`). The entry was instead verified through the 16-game trial: Elo 1,530 (6 wins, 8 draws, 2 losses).
