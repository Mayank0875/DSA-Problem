## Title
Fence Posts

## Slug
fence-posts

## Difficulty
Medium

## Description
Workers remove posts from an old fence.

The game involves posts numbered $1, 2, \dots, n$.
The game is played in turns, and Worker A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining posts.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the start post or the end post from the sequence. The game then continues with the other player.

Both Worker A and Worker B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of posts $n$.

## Examples

### 1

#### Input
1

#### Output
Worker A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Worker A removes 1. The remaining sequence is empty (XOR sum 0). Worker B cannot move and loses. Worker A wins.

### 2

#### Input
2

#### Output
Worker B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Worker A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Worker B will then remove the last number, leaving an empty sequence (XOR 0), causing Worker A to lose on the next turn. Worker B wins.

## Input Format
- The only input line has an integer n, the number of posts.

## Output Format
- Return "Worker A" if Worker A wins, or "Worker B" if Worker B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
