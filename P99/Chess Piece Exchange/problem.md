## Title
Chess Piece Exchange

## Slug
chess-piece-exchange

## Difficulty
Hard

## Description
Players capture pieces. The captured piece determines the next target square.

White and Black are playing a strategic game using a board state $p$ of length $n$. The game starts with a material advantage of 0.

The players take turns, with White moving first. On each turn, a player chooses an integer $x$ from the board state that has not been chosen before.
- If it is White's turn, the chosen value $x$ is **added** to the material advantage.
- If it is Black's turn, the chosen value $x$ is **subtracted** from the material advantage.

The rules for choosing $x$ are:
1. On the very first move of the game, White may choose **any** unselected piece from the board state.
2. On every move after the first:
   - Let $m$ be the index of the piece chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected piece.

The game continues until all pieces of the board state have been chosen.

White plays optimally to **maximize** the final material advantage, while Black plays optimally to **minimize** it.

Your task is to compute the final material advantage assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final material advantage is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final material advantage is 1.

## Input Format
- The first line contains an integer $n$ (length of board state).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final material advantage on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
