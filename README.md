# AI Sudoku Solver with Backtracking Visualization

![AI Sudoku Solver](https://img.shields.io/badge/Sudoku-Solver-blue)
![Algorithm](https://img.shields.io/badge/Algorithm-Backtracking-orange)
![HTML](https://img.shields.io/badge/HTML-5-red)
![CSS](https://img.shields.io/badge/CSS-3-blue)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)

A web-based Sudoku solver that visualizes the backtracking algorithm in action. Watch step-by-step as the AI works through the puzzle, testing different numbers and backtracking when necessary.

## Features

- **Interactive Sudoku Board**: Enter your own puzzles or load an example
- **Visualization Options**: 
  - Full auto-solve with adjustable speed
  - Step-by-step solving for educational purposes
- **Real-time Statistics**: Track attempts and backtracking operations
- **Visual Feedback**: Color-coded cells show the solving process:
  - Original numbers (gray)
  - Testing numbers (blue)
  - Backtracking (red)
  - Solved cells (green)
- **Responsive Design**: Works on desktop and mobile devices

## How It Works

This application implements the backtracking algorithm to solve Sudoku puzzles:

1. Find an empty cell on the board
2. Try placing a number (1-9) in that cell
3. Check if the placement is valid (follows Sudoku rules)
4. If valid, recursively attempt to fill the rest of the board
5. If the recursive call fails, backtrack (undo the choice) and try the next number
6. If all numbers fail, report that the puzzle has no solution

The visualization shows this process in real-time, allowing you to understand how backtracking algorithms work.

## How to Use

1. **Open the HTML file** in any modern web browser
2. **Input a Puzzle**: 
   - Enter numbers directly on the board
   - Or click "Load Example" to use a pre-defined puzzle
3. **Solve the Puzzle**:
   - Click "Solve" for automatic solving with visualization
   - Use "Step" to advance the solving process one step at a time
   - Adjust the speed slider to control visualization speed
4. **Other Controls**:
   - "Clear" to reset the board
   - "Stop" to halt the solving process

## Implementation Details

- **Pure JavaScript**: No external libraries or frameworks
- **CSS Grid**: Used for the Sudoku board layout
- **Async/Await**: For controlled visualization timing
- **Promise-based step mode**: For manual stepping through the algorithm

## Algorithm Performance

The backtracking algorithm has:
- **Time Complexity**: O(9^(n²)) in the worst case, where n is the board dimension (9x9)
- **Space Complexity**: O(n²) for the board representation

The statistics counter shows:
- **Attempts**: Number of cell value assignments tried
- **Backtracks**: Number of times the algorithm had to undo a choice

## Browser Compatibility

Tested and working on:
- Chrome 85+
- Firefox 80+
- Safari 14+
- Edge 85+

## Future Improvements

- Save/load puzzles from local storage
- Additional solving algorithms for comparison
- Puzzle generator with difficulty levels
- Board validation to ensure puzzles have unique solutions

## License

This project is open source and available under the MIT License.

## Acknowledgments

- Inspired by various Sudoku solving visualizations
- Built for educational purposes to demonstrate backtracking algorithms
