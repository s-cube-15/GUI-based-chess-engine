# 🎮 GUI-based Chess Engine

A fully-functional chess game built from scratch using Python and PyGame, featuring complete chess rule implementation, interactive GUI, and smooth animations.

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![PyGame](https://img.shields.io/badge/PyGame-2.x-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## 📋 Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [How to Play](#how-to-play)
- [Technical Implementation](#technical-implementation)
- [Project Structure](#project-structure)
- [Controls](#controls)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

### Core Chess Mechanics

- ♟️ **Complete Rule Implementation**: All standard chess rules including piece movements, captures, and turn-based gameplay
- 👑 **Special Moves**:
  - Pawn promotion (automatic queen promotion)
  - En passant captures
  - Castling (kingside and queenside)
- 🎯 **Game State Detection**: Real-time check, checkmate, and stalemate detection
- ✅ **Move Validation**: Prevents illegal moves and ensures king safety

### Interactive GUI

- 🎨 **Clean Visual Design**: 512x512 pixel board with alternating white/gray squares
- 🖱️ **Click-to-Move Interface**: Intuitive point-and-click piece selection and movement
- 💡 **Visual Feedback**:
  - Blue highlight on selected piece
  - Yellow highlights showing all valid moves for the selected piece
- 🎬 **Smooth Animations**: Fluid piece movement transitions at 60 FPS
- 📝 **Chess Notation**: Displays algebraic notation for each move in console

### Gameplay Features

- ⏮️ **Undo Move**: Press `Z` to undo the last move
- 🔄 **Reset Game**: Press `R` to start a new game
- 🏁 **Game Over Screen**: Clear victory/draw messages on game completion
- 📊 **Move History**: Complete move log tracking throughout the game

## 🎮 Demo

The game provides an interactive chess experience where players can:

- Practice chess strategies in a virtual environment
- Visualize and predict moves with highlighted valid squares
- Learn chess rules through real-time validation feedback
- Analyze gameplay with move history and undo functionality

## 🚀 Installation

### Prerequisites

- Python 3.x
- PyGame library

### Setup Steps

1. **Clone the repository**

   ```bash
   git clone https://github.com/s-cube-15/GUI-based-chess-engine.git
   cd GUI-based-chess-engine
   ```

2. **Install dependencies**

   ```bash
   pip install pygame
   ```

3. **Run the game**
   ```bash
   python ChessMain.py
   ```

## 🎯 How to Play

1. **Starting the Game**: Run `ChessMain.py` to launch the chess board
2. **Making Moves**:
   - Click on a piece to select it (blue highlight appears)
   - Valid move squares are highlighted in yellow
   - Click on a highlighted square to move the piece
   - Click the same piece again to deselect
3. **Special Moves**: The engine automatically handles pawn promotion, en passant, and castling when valid
4. **Game End**: The game detects and announces checkmate or stalemate

## 🔧 Technical Implementation

### Architecture

The project follows object-oriented design principles with three main components:

#### 1. **GameState Class** (`ChessEngine.py`)

- Manages the 8x8 board representation
- Tracks piece positions, turn order, and game status
- Implements move generation algorithms for all piece types
- Handles special move logic (castling rights, en passant)
- Detects check, checkmate, and stalemate conditions

#### 2. **Move Class** (`ChessEngine.py`)

- Encapsulates move information (start/end positions)
- Converts between array indices and chess notation
- Identifies special move types (promotion, en passant, castling)
- Provides move comparison and unique move ID generation

#### 3. **GUI Module** (`ChessMain.py`)

- Renders the game board and pieces using PyGame
- Handles user input (mouse clicks, keyboard commands)
- Implements move animations and visual highlights
- Manages game loop and display updates

### Key Algorithms

- **Move Generation**: Piece-specific movement patterns with boundary checking
- **Move Validation**: Simulates moves to prevent king exposure to check
- **Check Detection**: Analyzes opponent attacks on king position
- **Castling Logic**: Validates empty squares and no-check path requirements

## 📁 Project Structure

```
GUI-based-chess-engine/
├── ChessEngine.py      # Core game logic and rules
├── ChessMain.py        # GUI and game loop
├── images/             # Chess piece images (PNG format)
│   ├── wp.png         # White Pawn
│   ├── wR.png         # White Rook
│   ├── wN.png         # White Knight
│   ├── wB.png         # White Bishop
│   ├── wQ.png         # White Queen
│   ├── wK.png         # White King
│   ├── bp.png         # Black Pawn
│   ├── bR.png         # Black Rook
│   ├── bN.png         # Black Knight
│   ├── bB.png         # Black Bishop
│   ├── bQ.png         # Black Queen
│   └── bK.png         # Black King
└── README.md          # Project documentation
```

## ⌨️ Controls

| Key             | Action                   |
| --------------- | ------------------------ |
| **Mouse Click** | Select piece / Make move |
| **Z**           | Undo last move           |
| **R**           | Reset game (start new)   |

## 🚀 Future Enhancements

Potential improvements for future versions:

- [ ] AI opponent with minimax algorithm and alpha-beta pruning
- [ ] Difficulty levels (Easy, Medium, Hard)
- [ ] Move timer and clock
- [ ] Save/load game functionality
- [ ] Move history display on GUI
- [ ] Custom piece themes and board colors
- [ ] Sound effects for moves and captures
- [ ] PGN (Portable Game Notation) export
- [ ] Online multiplayer support
- [ ] Opening book integration

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

**Sudhanshu Sabale**

- GitHub: [@s-cube-15](https://github.com/s-cube-15)
- LinkedIn: [Sudhanshu Sabale](https://www.linkedin.com/in/sudhanshu-sabale-28ab4520a/)
- Email: sudhanshussable2@gmail.com

## 🙏 Acknowledgments

- Chess piece images sourced from open chess resources
- Built as a learning project to understand game development and chess algorithms
- Inspired by the classic game of chess and Python's versatility

---

⭐ **If you found this project helpful, please consider giving it a star!** ⭐
