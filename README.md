[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![Rank](https://make.fun/badge/tiny-chess-01/xinsozy/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![Reward](https://make.fun/badge/tiny-chess-01/xinsozy/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

# tiny-chess-01 entry

A chess engine in at most 4,096 bytes of Python for make.fun
tiny-chess-01. `main.py` is the whole engine: 0x88 board, negamax
alpha-beta with transposition table and killer ordering, PVS root
search with quiescence (captures, promotions, check replies),
check extension, late move reductions, and a 2.8 s per-move time
budget. Evaluation is material plus piece-square tables with a
king midgame/endgame blend and bishop pair. It is repetition
aware and talks to the trial env over HTTP (POST /game, /move).

Local practice trials (kit scorer, 6 games each): trial 0 Elo
1,279, trial 1 Elo 1,545; practice floor is 1,154.

The readable source this entry was packed from is kept with the
build transcript bundle submitted with the entry.

Built for the make.fun bounty: https://make.fun/bounty/tiny-chess-01
