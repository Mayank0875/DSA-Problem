## Title
Knight vs Pawn

## Slug
knight-vs-pawn

## Difficulty
Medium

## Description
A Knight jumps between squares. A Pawn walks. Pawns walk between squares that Knights don't jump between.

The chessboard has n squares numbered from 1 to n.
The Knight Moves connects specific pairs of squares with direct jumps.
The Pawn Moves is constructed based on a unique rule:
A direct step exists between two squares if and only if there is no jump connecting them.

Moving between any two connected squares takes exactly 1 hour on either network.
Two pieces, The Knight and The Pawn, depart from square 1 at the same time, heading for square n.

1. The Knight travels only using Knight Moves.
2. The Pawn travels only using Pawn Moves.

To ensure safety, they must never arrive at the same square at the same time (except for the final square n).
Your task is to compute the minimum number of hours required for **both** pieces to reach square n — specifically, the time when the slower piece arrives.
If either piece cannot reach square n using their respective network, return -1.

## Examples

### 1

#### Input
4 2
1 3
3 4

#### Output
2

#### Explanation
The smallest possible time is 2. One takes the direct route (1 hour), the other takes a path of length 2.

### 2

#### Input
4 6
1 2
1 3
1 4
2 3
2 4
3 4

#### Output
-1

#### Explanation
The graph is fully connected for one network, meaning the complement network has no edges. The second piece cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of squares and the number of jumps.
- The next m lines each contain two integers u and v, representing a jump between squares u and v.
- The graph is bidirectional. There is at most one jump between any pair of squares.

## Output Format
- Return a single integer representing the minimum hours required for the last piece to arrive. If it is impossible, return -1.

## Constraints
- 2 ≤ n ≤ 400
- 0 ≤ m ≤ n(n - 1)/2
- 1 ≤ u, v ≤ n
- u ≠ v

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
