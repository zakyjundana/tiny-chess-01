# tiny-chess-01

Deterministic Python 3.13 chess engine in ≤4096 bytes (stdlib only, no network, no file reads).

Alpha-beta search with quiescence, MVV-LVA ordering, killer/history moves, transposition table, and iterative deepening. Self-extracting: compressed payload embedded in main.py's own bytes.

Perft-verified on all 6 standard test positions to depth 3.

MIT License.
