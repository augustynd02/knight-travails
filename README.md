# Knight's Pathfinding Algorithm

## Methods

### `constructor()`
- Initializes the knight's adjacency list, representing all possible moves for each square on the chessboard.

### `#createAdjacencyList()`
- Generates the adjacency list for the chessboard, where each square's key maps to an array of all possible knight moves from that square.

### `#calculateKnightMoves(square)`
- Calculates all possible moves a knight can make from a given square.
- Filters out moves that are out of bounds (outside the 8x8 chessboard).

### `createPath(start, end)`
- Uses BFS to find the shortest path between a start and end square on the chessboard.
- Returns an array of squares representing the path from start to end.

## Usage

```javascript
const knight = new Knight();

// Find the shortest path between two squares (start and end)
const start = [0, 0];  // Starting square
const end = [7, 7];    // Ending square

const path = knight.createPath(start, end);

console.log(path); // Output: The shortest path as an array of squares
