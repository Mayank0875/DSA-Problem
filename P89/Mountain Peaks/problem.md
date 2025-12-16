## Title
Mountain Peaks

## Slug
mountain-peaks

## Difficulty
Medium

## Description
Climbers conquer peaks in a range.

The game involves peaks numbered $1, 2, \dots, n$.
The game is played in turns, and Climber 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining peaks.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the first peak or the last peak from the sequence. The game then continues with the other player.

Both Climber 1 and Climber 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of peaks $n$.

## Examples

### 1

#### Input
1

#### Output
Climber 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Climber 1 removes 1. The remaining sequence is empty (XOR sum 0). Climber 2 cannot move and loses. Climber 1 wins.

### 2

#### Input
2

#### Output
Climber 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Climber 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Climber 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Climber 1 to lose on the next turn. Climber 2 wins.

## Input Format
- The only input line has an integer n, the number of peaks.

## Output Format
- Return "Climber 1" if Climber 1 wins, or "Climber 2" if Climber 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
