# Connect 4 with Minimax Algorithm

This repository contains an implementation of the classic Connect 4 game enhanced with an AI opponent powered by the Minimax algorithm. The AI includes alpha-beta pruning for improved performance and strategic decision-making. A simple yet engaging graphical user interface (GUI) is implemented using Pygame.

<p align="center">
  <img src="https://github.com/Amir-rfz/Connect-4-Game-Bot/blob/main/result.gif" 
       alt="Result GIF" 
       style="width: 450px; border: 1px solid #ddd; border-radius: 8px;">
</p>
<p align="center" style="font-size: 14px; color: #555;">
  Result of the Minimax Algorithm with depth 5
</p>
<p align="center" style="font-size: 14px; color: #555;">
  Red is the agent and yellow is computer
</p>

## Features

- **Game Mechanics**: Classic Connect 4 game rules where two players (Human vs AI) take turns dropping pieces into a grid.
- **Minimax Algorithm**:
  - Depth-limited search for AI decision-making.
  - Alpha-beta pruning to optimize computational efficiency.
  - Configurable AI difficulty via adjustable depth.
- **Graphical User Interface**:
  - Colorful and responsive UI created with Pygame.
  - Displays game grid, moves, and winner announcement.
- **Dynamic AI Strategy**:
  - Combines deterministic Minimax moves with randomness for unpredictable gameplay.

## Requirements

- Python 3.x
- Pygame (`pip install pygame`)
- NumPy (`pip install numpy`)

## How It Works

### Minimax Algorithm
The AI uses the Minimax algorithm with alpha-beta pruning to evaluate all possible moves and choose the optimal one. The algorithm:
1. Explores possible game states up to a defined depth.
2. Scores each state based on the likelihood of winning.
3. Applies alpha-beta pruning to eliminate branches that cannot affect the final decision, saving computation time.

### Graphical User Interface
The game's GUI visualizes:
- The board's current state.
- Player and AI moves.
- A clear message announcing the winner or a draw.

### Adjustable Parameters
- **AI Depth**: Modify the `minimax_depth` parameter to control the AI's difficulty level.
- **Randomness**: Add randomness to the AI's moves by tweaking the `randomness_percent` parameter.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/connect4-minimax.git
   cd connect4-minimax
   ```

2. Install dependencies:
   ```bash
   pip install pygame numpy
   ```

3. Run the game:
   ```bash
   python connect4.py
   ```

## File Structure

- `connect4.py`: Main game implementation including the Minimax AI and Pygame UI.
- `README.md`: Project documentation.

## Contributing

Contributions are welcome! If you'd like to add features or fix issues, feel free to fork this repository and create a pull request.
