## Title
Traffic Jam

## Slug
traffic-jam

## Difficulty
Medium

## Description
Police clear cars from a traffic jam line.

The game involves cars numbered $1, 2, \dots, n$.
The game is played in turns, and Officer 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining cars.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the front car or the back car from the sequence. The game then continues with the other player.

Both Officer 1 and Officer 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of cars $n$.

## Examples

### 1

#### Input
1

#### Output
Officer 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Officer 1 removes 1. The remaining sequence is empty (XOR sum 0). Officer 2 cannot move and loses. Officer 1 wins.

### 2

#### Input
2

#### Output
Officer 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Officer 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Officer 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Officer 1 to lose on the next turn. Officer 2 wins.

## Input Format
- The only input line has an integer n, the number of cars.

## Output Format
- Return "Officer 1" if Officer 1 wins, or "Officer 2" if Officer 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
