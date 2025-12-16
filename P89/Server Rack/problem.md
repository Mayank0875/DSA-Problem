## Title
Server Rack

## Slug
server-rack

## Difficulty
Medium

## Description
Admins pull servers from a rack row.

The game involves servers numbered $1, 2, \dots, n$.
The game is played in turns, and Admin 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining servers.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the top server or the bottom server from the sequence. The game then continues with the other player.

Both Admin 1 and Admin 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of servers $n$.

## Examples

### 1

#### Input
1

#### Output
Admin 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Admin 1 removes 1. The remaining sequence is empty (XOR sum 0). Admin 2 cannot move and loses. Admin 1 wins.

### 2

#### Input
2

#### Output
Admin 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Admin 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Admin 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Admin 1 to lose on the next turn. Admin 2 wins.

## Input Format
- The only input line has an integer n, the number of servers.

## Output Format
- Return "Admin 1" if Admin 1 wins, or "Admin 2" if Admin 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
