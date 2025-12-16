## Title
Sushi Conveyor

## Slug
sushi-conveyor

## Difficulty
Medium

## Description
Customers take plates from a straight conveyor belt.

The game involves plates numbered $1, 2, \dots, n$.
The game is played in turns, and Eater 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining plates.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the first plate or the last plate from the sequence. The game then continues with the other player.

Both Eater 1 and Eater 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of plates $n$.

## Examples

### 1

#### Input
1

#### Output
Eater 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Eater 1 removes 1. The remaining sequence is empty (XOR sum 0). Eater 2 cannot move and loses. Eater 1 wins.

### 2

#### Input
2

#### Output
Eater 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Eater 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Eater 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Eater 1 to lose on the next turn. Eater 2 wins.

## Input Format
- The only input line has an integer n, the number of plates.

## Output Format
- Return "Eater 1" if Eater 1 wins, or "Eater 2" if Eater 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
