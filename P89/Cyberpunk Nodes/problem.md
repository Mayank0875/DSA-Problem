## Title
Cyberpunk Nodes

## Slug
cyberpunk-nodes

## Difficulty
Medium

## Description
Netrunners hack nodes in a linear network.

The game involves nodes numbered $1, 2, \dots, n$.
The game is played in turns, and Runner 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining nodes.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the entry node or the exit node from the sequence. The game then continues with the other player.

Both Runner 1 and Runner 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of nodes $n$.

## Examples

### 1

#### Input
1

#### Output
Runner 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Runner 1 removes 1. The remaining sequence is empty (XOR sum 0). Runner 2 cannot move and loses. Runner 1 wins.

### 2

#### Input
2

#### Output
Runner 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Runner 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Runner 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Runner 1 to lose on the next turn. Runner 2 wins.

## Input Format
- The only input line has an integer n, the number of nodes.

## Output Format
- Return "Runner 1" if Runner 1 wins, or "Runner 2" if Runner 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
