# Lux Chess

**Lux Chess** is a Unity chess game built from scratch using only C#.
This makes the code easy to edit, debug and understand, but it is not as fast as commercially produced chess engines written in
written in C or C++.

Made during the winter of 2015.

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/y2XRnRherwk/0.jpg)](https://www.youtube.com/watch?v=y2XRnRherwk)

## Table of Contents
- [Features](#features)
- [Getting Started](#getting-started)
- [To-Do](#to-do)
- [AI](#ai)
- [References](#references)
- [License](#license)

## Features
- **Single Player Mode**: Play against the AI, can you beat it?
- **Customizable Boards and Pieces**: You can customize the king and his army as you like.
- **Undo/Redo**: Doesn't matter if you make mistake :)
- **Save and Load**: Save or import games using the FEN (Forsyth-Edwards Notation).
- **Efficient move generation**: Utilizes bitboards for quick and efficient chess representation.

## Getting Started

### Installation

1. Clone the repository
2. Open inside of Unity
3. Play


## TO-DO

- Rewrite the code to use Unity Burst compiler
- Add Multiplayer
- Add Opening book


## AI

By default, the AI has a limited amount of time to think, a few seconds, after which it stops. This results in an average depth of 5-7 moves,
which is low compared to 10+ moves in more optimised engines.
The AI uses alpha-beta pruning of the search tree to reduce the number of nodes evaluated by the
minimax algorithm.  
To further improve performance, the AI also has Zobrist hashing and PV table.

## References

- https://www.chessprogramming.org
- https://en.wikipedia.org/wiki/Forsyth%E2%80%93Edwards_Notatio
- https://en.wikipedia.org/wiki/Alpha%E2%80%93beta_pruning
- https://en.wikipedia.org/wiki/Minimax#Minimax_algorithm_with_alternate_moves
- https://tearth.dev/bitboard-viewer/

## License

This project is licensed under the MIT License - see the LICENSE file for details.