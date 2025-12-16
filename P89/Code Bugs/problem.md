## Title
Code Bugs

## Slug
code-bugs

## Difficulty
Medium

## Description
Developers fix bugs listed in a tracker.

The game involves bugs numbered $1, 2, \dots, n$.
The game is played in turns, and Dev A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining bugs.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the top bug or the bottom bug from the sequence. The game then continues with the other player.

Both Dev A and Dev B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of bugs $n$.

## Examples

### 1

#### Input
1

#### Output
Dev A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Dev A removes 1. The remaining sequence is empty (XOR sum 0). Dev B cannot move and loses. Dev A wins.

### 2

#### Input
2

#### Output
Dev B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Dev A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Dev B will then remove the last number, leaving an empty sequence (XOR 0), causing Dev A to lose on the next turn. Dev B wins.

## Input Format
- The only input line has an integer n, the number of bugs.

## Output Format
- Return "Dev A" if Dev A wins, or "Dev B" if Dev B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
