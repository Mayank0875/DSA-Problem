## Title
DNA Sequencing

## Slug
dna-sequencing

## Difficulty
Medium

## Description
Scientists remove base pairs from a DNA strand.

The game involves base pairs numbered $1, 2, \dots, n$.
The game is played in turns, and Scientist A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining base pairs.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the 5' end or the 3' end from the sequence. The game then continues with the other player.

Both Scientist A and Scientist B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of base pairs $n$.

## Examples

### 1

#### Input
1

#### Output
Scientist A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Scientist A removes 1. The remaining sequence is empty (XOR sum 0). Scientist B cannot move and loses. Scientist A wins.

### 2

#### Input
2

#### Output
Scientist B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Scientist A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Scientist B will then remove the last number, leaving an empty sequence (XOR 0), causing Scientist A to lose on the next turn. Scientist B wins.

## Input Format
- The only input line has an integer n, the number of base pairs.

## Output Format
- Return "Scientist A" if Scientist A wins, or "Scientist B" if Scientist B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
