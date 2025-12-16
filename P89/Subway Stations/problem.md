## Title
Subway Stations

## Slug
subway-stations

## Difficulty
Medium

## Description
Inspectors close stations on a line.

The game involves stations numbered $1, 2, \dots, n$.
The game is played in turns, and Inspector A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining stations.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the start station or the end station from the sequence. The game then continues with the other player.

Both Inspector A and Inspector B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of stations $n$.

## Examples

### 1

#### Input
1

#### Output
Inspector A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Inspector A removes 1. The remaining sequence is empty (XOR sum 0). Inspector B cannot move and loses. Inspector A wins.

### 2

#### Input
2

#### Output
Inspector B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Inspector A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Inspector B will then remove the last number, leaving an empty sequence (XOR 0), causing Inspector A to lose on the next turn. Inspector B wins.

## Input Format
- The only input line has an integer n, the number of stations.

## Output Format
- Return "Inspector A" if Inspector A wins, or "Inspector B" if Inspector B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
