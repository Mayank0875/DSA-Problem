## Title
Fighter Jets

## Slug
fighter-jets

## Difficulty
Medium

## Description
Pilots peel off from a formation flight.

The game involves jets numbered $1, 2, \dots, n$.
The game is played in turns, and Pilot A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining jets.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the lead jet or the rear jet from the sequence. The game then continues with the other player.

Both Pilot A and Pilot B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of jets $n$.

## Examples

### 1

#### Input
1

#### Output
Pilot A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Pilot A removes 1. The remaining sequence is empty (XOR sum 0). Pilot B cannot move and loses. Pilot A wins.

### 2

#### Input
2

#### Output
Pilot B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Pilot A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Pilot B will then remove the last number, leaving an empty sequence (XOR 0), causing Pilot A to lose on the next turn. Pilot B wins.

## Input Format
- The only input line has an integer n, the number of jets.

## Output Format
- Return "Pilot A" if Pilot A wins, or "Pilot B" if Pilot B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
