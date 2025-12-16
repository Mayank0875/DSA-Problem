## Title
Potion Bottles

## Slug
potion-bottles

## Difficulty
Medium

## Description
Alchemists use ingredients from a shelf of potions.

The game involves bottles numbered $1, 2, \dots, n$.
The game is played in turns, and Alchemist 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining bottles.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left bottle or the right bottle from the sequence. The game then continues with the other player.

Both Alchemist 1 and Alchemist 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of bottles $n$.

## Examples

### 1

#### Input
1

#### Output
Alchemist 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Alchemist 1 removes 1. The remaining sequence is empty (XOR sum 0). Alchemist 2 cannot move and loses. Alchemist 1 wins.

### 2

#### Input
2

#### Output
Alchemist 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Alchemist 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Alchemist 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Alchemist 1 to lose on the next turn. Alchemist 2 wins.

## Input Format
- The only input line has an integer n, the number of bottles.

## Output Format
- Return "Alchemist 1" if Alchemist 1 wins, or "Alchemist 2" if Alchemist 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
