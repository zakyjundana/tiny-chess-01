# tiny-chess-01

Deterministic Python 3.13 chess engine in ≤4096 bytes (stdlib only, no network, no file reads).

Alpha-beta search with quiescence, MVV-LVA ordering, killer/history moves, transposition table, and iterative deepening. Self-extracting: compressed payload embedded in main.py's own bytes.

Perft-verified on all 6 standard test positions to depth 3.

## Build

`main.py` is produced by `tools/build_main.py` from `src/engine.py`: LZMA preset 9|extreme, base85-encoded, self-extracting header.

MIT License.

## Usage

Run main.py directly (Python 3.13):

    python3 main.py

The engine plays a full game with legal move generation, check detection, and
basic alpha-beta search. No third-party packages required.

