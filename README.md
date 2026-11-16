# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Oxim97-byte/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Oxim97-byte/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

Bitboard chess engine in 4,096 bytes of Python. All move generation and attack detection run on Python big-int bitwise ops (C speed); slider attacks use the first-blocker ray trick, no magic tables. Search is PVS + transposition table + killer moves + LMR + null-move pruning + quiescence, to a fixed node budget (deterministic, no clock). Evaluation is material + mirrored piece-square tables + bishop pair + passed pawns, with material and PST tracked incrementally. The readable source is packed with LZMA via the kit's `makefun compress`.

## Run it

```sh
python3 main.py
```

---

Entered on [make.fun](https://make.fun/?ref={referral_code}&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
