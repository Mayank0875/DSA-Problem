## Title
Laser Beams

## Slug
laser-beams

## Difficulty
Medium

## Description
Technicians disable laser beams in a corridor.

The game involves beams numbered $1, 2, \dots, n$.
The game is played in turns, and Agent 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining beams.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the front beam or the back beam from the sequence. The game then continues with the other player.

Both Agent 1 and Agent 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of beams $n$.

## Examples

### 1

#### Input
1

#### Output
Agent 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Agent 1 removes 1. The remaining sequence is empty (XOR sum 0). Agent 2 cannot move and loses. Agent 1 wins.

### 2

#### Input
2

#### Output
Agent 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Agent 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Agent 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Agent 1 to lose on the next turn. Agent 2 wins.

## Input Format
- The only input line has an integer n, the number of beams.

## Output Format
- Return "Agent 1" if Agent 1 wins, or "Agent 2" if Agent 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
