## Title
Energy Cell Depletion

## Slug
energy-cell-depletion

## Difficulty
Medium

## Description
Engineers disable energy cells in a reactor core.

The game involves cells numbered $1, 2, \dots, n$.
The game is played in turns, and Engineer X always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining cells.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left cell or the right cell from the sequence. The game then continues with the other player.

Both Engineer X and Engineer Y are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of cells $n$.

## Examples

### 1

#### Input
1

#### Output
Engineer X

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Engineer X removes 1. The remaining sequence is empty (XOR sum 0). Engineer Y cannot move and loses. Engineer X wins.

### 2

#### Input
2

#### Output
Engineer Y

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Engineer X can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Engineer Y will then remove the last number, leaving an empty sequence (XOR 0), causing Engineer X to lose on the next turn. Engineer Y wins.

## Input Format
- The only input line has an integer n, the number of cells.

## Output Format
- Return "Engineer X" if Engineer X wins, or "Engineer Y" if Engineer Y wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
