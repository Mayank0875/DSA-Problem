## Title
Crystal Shards

## Slug
crystal-shards

## Difficulty
Medium

## Description
Sorcerers collect shards from a magical formation.

The game involves shards numbered $1, 2, \dots, n$.
The game is played in turns, and Sorcerer 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining shards.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left shard or the right shard from the sequence. The game then continues with the other player.

Both Sorcerer 1 and Sorcerer 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of shards $n$.

## Examples

### 1

#### Input
1

#### Output
Sorcerer 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Sorcerer 1 removes 1. The remaining sequence is empty (XOR sum 0). Sorcerer 2 cannot move and loses. Sorcerer 1 wins.

### 2

#### Input
2

#### Output
Sorcerer 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Sorcerer 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Sorcerer 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Sorcerer 1 to lose on the next turn. Sorcerer 2 wins.

## Input Format
- The only input line has an integer n, the number of shards.

## Output Format
- Return "Sorcerer 1" if Sorcerer 1 wins, or "Sorcerer 2" if Sorcerer 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
