## Title
Treasure Chests

## Slug
treasure-chests

## Difficulty
Medium

## Description
Pirates loot chests lined up on a deck.

The game involves chests numbered $1, 2, \dots, n$.
The game is played in turns, and Pirate A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining chests.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left chest or the right chest from the sequence. The game then continues with the other player.

Both Pirate A and Pirate B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of chests $n$.

## Examples

### 1

#### Input
1

#### Output
Pirate A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Pirate A removes 1. The remaining sequence is empty (XOR sum 0). Pirate B cannot move and loses. Pirate A wins.

### 2

#### Input
2

#### Output
Pirate B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Pirate A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Pirate B will then remove the last number, leaving an empty sequence (XOR 0), causing Pirate A to lose on the next turn. Pirate B wins.

## Input Format
- The only input line has an integer n, the number of chests.

## Output Format
- Return "Pirate A" if Pirate A wins, or "Pirate B" if Pirate B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
