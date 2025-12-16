## Title
Satellite Array

## Slug
satellite-array

## Difficulty
Medium

## Description
Operators decommission satellites in an orbital line.

The game involves satellites numbered $1, 2, \dots, n$.
The game is played in turns, and Operator 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining satellites.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the west sat or the east sat from the sequence. The game then continues with the other player.

Both Operator 1 and Operator 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of satellites $n$.

## Examples

### 1

#### Input
1

#### Output
Operator 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Operator 1 removes 1. The remaining sequence is empty (XOR sum 0). Operator 2 cannot move and loses. Operator 1 wins.

### 2

#### Input
2

#### Output
Operator 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Operator 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Operator 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Operator 1 to lose on the next turn. Operator 2 wins.

## Input Format
- The only input line has an integer n, the number of satellites.

## Output Format
- Return "Operator 1" if Operator 1 wins, or "Operator 2" if Operator 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
