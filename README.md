# tiny-chess-01

An original compact chess engine in 4 KB of Python, built for the
make.fun "Build the strongest chess engine in 4 KB of Python" bounty.

## Engine

- 0x88 board, alpha-beta search with PVS and iterative deepening
- Transposition table, killer moves, MVV-LVA move ordering
- Quiescence over captures/promotions and replies to check
- Piece-square evaluation with tapered king and bishop pair
- Fixed node budget per move (250,000 nodes) — deterministic: no clock
  and no unseeded randomness, so replays play the same moves
- `main.py` holds the engine lzma-compressed and unpacks it at run time
  (compression is allowed and counted toward the 4,096-byte cap)

## Links

- Bounty: https://make.fun/bounty/tiny-chess-01
- Built with [make.fun](https://make.fun?ref=xc4ppx8f)
