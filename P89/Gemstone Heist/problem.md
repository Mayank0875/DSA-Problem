## Title
Gemstone Heist

## Slug
gemstone-heist

## Difficulty
Medium

## Description
Thieves take turns stealing gems from a display case.

The game involves gems numbered $1, 2, \dots, n$.
The game is played in turns, and Thief A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining gems.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left gem or the right gem from the sequence. The game then continues with the other player.

Both Thief A and Thief B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of gems $n$.

## Examples

### 1

#### Input
1

#### Output
Thief A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Thief A removes 1. The remaining sequence is empty (XOR sum 0). Thief B cannot move and loses. Thief A wins.

### 2

#### Input
2

#### Output
Thief B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Thief A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Thief B will then remove the last number, leaving an empty sequence (XOR 0), causing Thief A to lose on the next turn. Thief B wins.

## Input Format
- The only input line has an integer n, the number of gems.

## Output Format
- Return "Thief A" if Thief A wins, or "Thief B" if Thief B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
