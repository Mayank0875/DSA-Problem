## Title
Flower Bed

## Slug
flower-bed

## Difficulty
Medium

## Description
Gardeners pick flowers from a row.

The game involves flowers numbered $1, 2, \dots, n$.
The game is played in turns, and Gardener A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining flowers.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left flower or the right flower from the sequence. The game then continues with the other player.

Both Gardener A and Gardener B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of flowers $n$.

## Examples

### 1

#### Input
1

#### Output
Gardener A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Gardener A removes 1. The remaining sequence is empty (XOR sum 0). Gardener B cannot move and loses. Gardener A wins.

### 2

#### Input
2

#### Output
Gardener B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Gardener A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Gardener B will then remove the last number, leaving an empty sequence (XOR 0), causing Gardener A to lose on the next turn. Gardener B wins.

## Input Format
- The only input line has an integer n, the number of flowers.

## Output Format
- Return "Gardener A" if Gardener A wins, or "Gardener B" if Gardener B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
