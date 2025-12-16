## Title
Neon Signs

## Slug
neon-signs

## Difficulty
Medium

## Description
Repairmen fix letters on a neon sign.

The game involves letters numbered $1, 2, \dots, n$.
The game is played in turns, and Repairman 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining letters.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the first letter or the last letter from the sequence. The game then continues with the other player.

Both Repairman 1 and Repairman 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of letters $n$.

## Examples

### 1

#### Input
1

#### Output
Repairman 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Repairman 1 removes 1. The remaining sequence is empty (XOR sum 0). Repairman 2 cannot move and loses. Repairman 1 wins.

### 2

#### Input
2

#### Output
Repairman 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Repairman 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Repairman 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Repairman 1 to lose on the next turn. Repairman 2 wins.

## Input Format
- The only input line has an integer n, the number of letters.

## Output Format
- Return "Repairman 1" if Repairman 1 wins, or "Repairman 2" if Repairman 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
