## Knight's Travails

This project is a JavaScript implementation of the classic Knight's Travails problem. It uses breadth-first search to compute the shortest possible route a knight can take on a standard 8x8 chessboard from one square to another.

---

### Project Description

The Knight's Travails challenge is about finding the minimum number of moves required for a knight to travel from a starting square to a target square. This project:

- Models the board as an implicit graph.
- Generates valid knight moves for any square.
- Uses breadth-first search to guarantee the shortest path.
- Tracks visited positions to prevent revisiting nodes.
- Reconstructs the full route using parent pointers.

---

### Features

- Validates input for out-of-bounds positions and identical starting and ending squares.
- Generates neighboring squares according to standard knight movement rules.
- Uses efficient queue-based traversal to minimize unnecessary work.
- Reconstructs a path cleanly from the target back to the source.
- Prints the final route and total number of moves in a simple format.

---

### Concepts Applied

- Graph traversal with breadth-first search
- Implicit graph modeling
- Queue-based algorithm design
- Position encoding for path reconstruction
- Defensive programming through input validation

---

### Usage

To use this logic in a script:

```javascript
const knights = new KnightsTravails();
knights.knightMoves([7, 7], [3, 0]);
```

Example output:

```
You made it in 3 moves! Here's your path:
[7,7] => [6,5] => [5,3] => [3,0]
```