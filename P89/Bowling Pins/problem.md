## Title
Bowling Pins

## Slug
bowling-pins

## Difficulty
Medium

## Description
Players knock down pins lined up in a row.

The game involves pins numbered $1, 2, \dots, n$.
The game is played in turns, and Bowler A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining pins.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left pin or the right pin from the sequence. The game then continues with the other player.

Both Bowler A and Bowler B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of pins $n$.

## Examples

### 1

#### Input
1

#### Output
Bowler A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Bowler A removes 1. The remaining sequence is empty (XOR sum 0). Bowler B cannot move and loses. Bowler A wins.

### 2

#### Input
2

#### Output
Bowler B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Bowler A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Bowler B will then remove the last number, leaving an empty sequence (XOR 0), causing Bowler A to lose on the next turn. Bowler B wins.

## Input Format
- The only input line has an integer n, the number of pins.

## Output Format
- Return "Bowler A" if Bowler A wins, or "Bowler B" if Bowler B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
