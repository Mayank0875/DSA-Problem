## Title
Asteroid Belt

## Slug
asteroid-belt

## Difficulty
Medium

## Description
Miners extract ore from asteroids in a belt.

The game involves asteroids numbered $1, 2, \dots, n$.
The game is played in turns, and Miner 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining asteroids.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left asteroid or the right asteroid from the sequence. The game then continues with the other player.

Both Miner 1 and Miner 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of asteroids $n$.

## Examples

### 1

#### Input
1

#### Output
Miner 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Miner 1 removes 1. The remaining sequence is empty (XOR sum 0). Miner 2 cannot move and loses. Miner 1 wins.

### 2

#### Input
2

#### Output
Miner 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Miner 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Miner 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Miner 1 to lose on the next turn. Miner 2 wins.

## Input Format
- The only input line has an integer n, the number of asteroids.

## Output Format
- Return "Miner 1" if Miner 1 wins, or "Miner 2" if Miner 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
