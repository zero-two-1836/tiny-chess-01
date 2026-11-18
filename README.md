[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/zero-two-1836/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/zero-two-1836/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

# tiny-chess-01

A strong chess engine in 4 KB of Python. `main.py` is the packed entrypoint
(the makefun-compress/v1 stub around an LZMA stream of `engine.py`).
Runs standalone: `MAKEFUN_ENV_URL=<env> python3 main.py`.

Engine: 0x88 board, negamax alpha-beta with transposition table, killer moves,
quiescence, PVS, null-move pruning and late-move reductions, iterative
deepening to a fixed 60,000-node budget. Deterministic, stdlib only.
