## Title
Chess Pieces

## Slug
chess-pieces

## Difficulty
Medium

## Description
Players capture pieces lined up on the board edge.

The game involves pieces numbered $1, 2, \dots, n$.
The game is played in turns, and White always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining pieces.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left piece or the right piece from the sequence. The game then continues with the other player.

Both White and Black are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of pieces $n$.

## Examples

### 1

#### Input
1

#### Output
White

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. White removes 1. The remaining sequence is empty (XOR sum 0). Black cannot move and loses. White wins.

### 2

#### Input
2

#### Output
Black

#### Explanation
The sequence is [1, 2]. XOR sum is 3. White can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Black will then remove the last number, leaving an empty sequence (XOR 0), causing White to lose on the next turn. Black wins.

## Input Format
- The only input line has an integer n, the number of pieces.

## Output Format
- Return "White" if White wins, or "Black" if Black wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
