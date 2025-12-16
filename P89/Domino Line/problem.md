## Title
Domino Line

## Slug
domino-line

## Difficulty
Medium

## Description
Players take dominoes from the ends of a line.

The game involves dominoes numbered $1, 2, \dots, n$.
The game is played in turns, and Player 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining dominoes.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left domino or the right domino from the sequence. The game then continues with the other player.

Both Player 1 and Player 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of dominoes $n$.

## Examples

### 1

#### Input
1

#### Output
Player 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Player 1 removes 1. The remaining sequence is empty (XOR sum 0). Player 2 cannot move and loses. Player 1 wins.

### 2

#### Input
2

#### Output
Player 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Player 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Player 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Player 1 to lose on the next turn. Player 2 wins.

## Input Format
- The only input line has an integer n, the number of dominoes.

## Output Format
- Return "Player 1" if Player 1 wins, or "Player 2" if Player 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
