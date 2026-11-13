# tiny-chess-01 entry

Chess engine for the make.fun tiny-chess-01 competition, built to fit
the 4 KB Python size limit. `main.py` is the whole engine: it plays
every game through the make.fun env using only the Python standard
library, and reads no other file in this repository.

Engine: 0x88 board, alpha-beta + quiescence search, transposition
table, killer moves, MVV-LVA ordering, null-move pruning and LMR,
formula piece-square tables + bishop pair, fixed 60,000-node budget
per move (deterministic). Practice Elo ~1246 across the kit's three
trial gauntlets. `main.py` is packed from the readable `engine.py`
with the kit's `makefun compress`.

MIT licensed. See `LICENSE`.
