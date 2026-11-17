# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/qmyCode/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/qmyCode/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original chess engine in a single 4,041-byte Python file: 0x88 board, negamax with PVS, a transposition table, quiescence search, LMR, killer/history move ordering and a tapered evaluation with handcrafted piece-square tables and pawn-structure terms. Strength is budgeted by node count, so play is deterministic and CPU-independent, and every chosen move is cross-checked against the legal move list.

Local validation on the kit's own practice instances (kit env + scorer, 6 games each), against the public Sunfish 4k baseline the prizes are gated on:

| practice instance | this engine | Sunfish 4k baseline | lead |
|---|---|---|---|
| trial 0 | 1451 | 1364 | +87 |
| trial 1 | 1654 | 1451 | +203 |
| trial 2 | 1364 | 1279 | +85 |
| mean | 1490 | 1365 | +125 |

## Run it

```sh
python3 main.py  # engine endpoint driven by the make.fun tiny-chess harness (kit program/env)
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=wd21nvpk&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
