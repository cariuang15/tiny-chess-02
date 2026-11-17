# tiny-chess-02

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/cariuang15/tiny-chess-02/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/cariuang15/tiny-chess-02/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB Python chess engine for make.fun's "Build the strongest chess
engine in 4 KB of Python" bounty ($500 in USDC, 20 places paid). Pure
standard library: 0x88 board, negamax + alpha-beta with PVS, LMR and
null-move pruning, quiescence search (captures and promotions),
repetition detection in search, transposition table, MVV-LVA + killer
ordering, and a richer eval (passed pawns, isolated pawns, rook on the
7th, phase-interpolated king table). Fixed 100,000-node budget per move
(deterministic, ~1.5–3.3 s/move). Practice Elo 1,578 over 18 games
(14 wins, 0 draws, 4 losses — all wins by checkmate). `main.py` is
3,343 bytes (an LZMA-packed payload produced by `makefun compress`
from the readable engine source).

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=csc1bejp&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>

## Submit

Push only `main.py`, `LICENSE`, `README.md` (repo ≤ 8,192 bytes total).
Badge URLs use the real GitHub owner/repo (`cariuang15` / `tiny-chess-02`)
and the referral link uses the make.fun referral code `csc1bejp`. Then run
`grade-local` (needs Node.js + Docker) and submit the repo on
https://make.fun/bounty/tiny-chess-01 before 24 Nov 2026 17:00 UTC.
