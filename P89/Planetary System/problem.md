## Title
Planetary System

## Slug
planetary-system

## Difficulty
Medium

## Description
Aliens harvest planets from a solar system line.

The game involves planets numbered $1, 2, \dots, n$.
The game is played in turns, and Alien X always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining planets.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the inner planet or the outer planet from the sequence. The game then continues with the other player.

Both Alien X and Alien Y are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of planets $n$.

## Examples

### 1

#### Input
1

#### Output
Alien X

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Alien X removes 1. The remaining sequence is empty (XOR sum 0). Alien Y cannot move and loses. Alien X wins.

### 2

#### Input
2

#### Output
Alien Y

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Alien X can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Alien Y will then remove the last number, leaving an empty sequence (XOR 0), causing Alien X to lose on the next turn. Alien Y wins.

## Input Format
- The only input line has an integer n, the number of planets.

## Output Format
- Return "Alien X" if Alien X wins, or "Alien Y" if Alien Y wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
