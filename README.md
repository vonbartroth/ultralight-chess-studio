<img width="607" height="679" alt="UCS" src="https://github.com/user-attachments/assets/8c87f6e2-fcc7-430d-bca1-9df53e23452e" />
# ultralight-chess-studio
Fast, zero-bloat native C++ chess GUI and engine suite for Linux and Windows XP - Windows 11

# Ultralight Chess Studio

A fast, zero-bloat native C++ chess GUI and engine suite built with **FLTK**, designed to run instantaneously on both **modern Linux** and **Windows XP / 7 / 10 / 11**.

*Designed for [Lichess puzzles, by ECO](https://cshancock.netlify.app/post/2021-06-23-lichess-puzzles-by-eco/)*

## Download & Run
Download the release package for your platform from the **[Releases](../../releases)** page, extract the archive, and launch the executable directly—no installation or runtime dependencies required:

* **Linux (x86_64):** Extract `UltralightChessStudio-v1.0-linux-x86_64.tar.gz` and run `./ultralight_chess`
* **Windows (XP / 7 / 10 / 11):** Extract `UltralightChessStudio-v1.0-win32-xp.zip` and run `UltralightChessStudio.exe`

*(Keep `pieces/`, `openings/`, `puzzles/`, `Book.bin`, and the engine executables `1850` and `stockfish` in the same folder as the main binary.)*

## Features
- **Double-Buffered Board (`604×676`):** Zero-flicker rendering with smooth drag-and-drop and click-to-move support.
- **7 Classic Board Color Themes:** Cycle through Classic Brown, Fritz Hiarcs, Azure Blue, Steel Blue, Fritz Nimzo, Fritz Cool, and Tournament Gray with one click.
- **Dual-Engine UCI Support:**
  - **1850:** Built-in PeSTO-based sparring engine with adjustable skill levels (`L1`–`L20`).
  - **Stockfish 11 (`SF`):** Infinite analysis engine (`Eng`) with live depth, centipawn/mate evaluation, and SAN principal variation.
- **Polyglot Opening Book (`Book.bin`):** Automatic book moves during play plus a live Book Explorer window showing candidate moves and weights.
- **ECO Opening Detection:** Live ECO code and opening title recognition as you play or step through games.
- **Multi-File PGN Memory & Standard PGN Export:** Remembers your exact last-visited game/puzzle index across up to 100 PGN files (`pgn_history.txt`) and exports clean 7-tag standard PGNs.
- **Tactics Puzzle Mode (`Puzzles`):** Load any PGN puzzle pack (such as Lichess Puzzles by ECO) for rapid auto-advancing tactical training.
- **Clipboard-Aware FEN Tools (`pFEN` / `cFEN`):** Auto-fills FEN strings from your clipboard with right-click mouse Paste/Clear support.

## Included Sample Puzzles & More Packs
A small sample files  and guide (`puzzles/README.txt`) are included so you can test **Puzzles** mode immediately.
* **Download More Puzzles (1.6+ Million by ECO):** Get the full collection of Lichess puzzles here https://cshancock.netlify.app/post/2021-06-23-lichess-puzzles-by-eco/ CC0 Public Domain).
* **Tip (Filtering by ELO Rating):** It is helpful to sort large ECO files by ELO rating and copy your desired rating range into a custom PGN file. **Lucas Chess** does this easily via `Tools > PGN viewer > Read PGN`—click the **Rating** column to sort, select your preferred range, and save.

## Controls & Shortcuts
- **Move Pieces:** Drag & drop or click origin and destination squares.
- **Step Through Moves:** `Left` / `Right` arrow keys, mouse wheel scroll, or `@<-` / `@->` buttons.
- **Paste FEN:** Right-click inside the FEN box for `Paste` / `Clear`, or press `Ctrl+V`.
- **About & Credits:** Press `F1`.

## License & Third-Party Notices
* **Ultralight Chess Studio & 1850 Engine:** Copyright © 2026 vonbartroth. Freeware for personal use; binary redistribution only.
* **Stockfish 11:** Created by T. Romstad, M. Costalba, J. Kiiski, G. Linscott, and the Stockfish developers. Stockfish is distributed as a separate external UCI executable under the **GNU General Public License v3.0 (GPLv3)** (see `Stockfish_GPLv3_Copying.txt` included in the release archive). The unmodified Stockfish 11 source code is available at [official-stockfish/Stockfish (sf_11)](https://github.com).
* **FLTK (Fast Light Toolkit):** Statically linked under the FLTK Library License (LGPLv2 with static linking exception).
