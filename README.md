# Dammen — International Draughts

A full-size **10×10 International Draughts** (dammen) game implementing the official FMJD rules, playable in the browser with no dependencies.

## Play

Open `index.html` in any browser. Two players share the mouse: click one of your highlighted pieces, then click a destination dot. Green dots are quiet moves, red dots are captures.

## Rules implemented

- 10×10 board, 20 pieces per side on the dark squares; White moves first.
- Men move one square diagonally forward, but **capture both forwards and backwards**.
- **Capturing is mandatory**, and the **maximum-capture (majority) rule** applies: you must play a sequence that captures the greatest possible number of pieces.
- Multi-jump sequences: captured pieces stay on the board (blocking further jumps) until the sequence ends, and no piece may be jumped twice.
- **Flying kings**: a king moves any distance along a diagonal, captures a piece at any distance, and may land on any empty square beyond it — including changing direction mid-sequence.
- A man promotes to a king only when its move **ends** on the far row; passing through the back row mid-capture does not promote.
- A player with no legal move (no pieces, or all blocked) loses.

## Features

- Legal-move highlighting with capture indication
- Mandatory-capture messages showing the required capture count
- Move history in standard 1–50 draughts notation
- Undo and New Game
- Last-move highlighting, piece counts, responsive board
