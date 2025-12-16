## Title
Ant Colony Tunnel

## Slug
ant-colony-tunnel

## Difficulty
Medium

## Description
Ants clear debris from a tunnel.

The game involves debris chunks numbered $1, 2, \dots, n$.
The game is played in turns, and Ant 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining debris chunks.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the entrance chunk or the deep chunk from the sequence. The game then continues with the other player.

Both Ant 1 and Ant 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of debris chunks $n$.

## Examples

### 1

#### Input
1

#### Output
Ant 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Ant 1 removes 1. The remaining sequence is empty (XOR sum 0). Ant 2 cannot move and loses. Ant 1 wins.

### 2

#### Input
2

#### Output
Ant 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Ant 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Ant 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Ant 1 to lose on the next turn. Ant 2 wins.

## Input Format
- The only input line has an integer n, the number of debris chunks.

## Output Format
- Return "Ant 1" if Ant 1 wins, or "Ant 2" if Ant 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
