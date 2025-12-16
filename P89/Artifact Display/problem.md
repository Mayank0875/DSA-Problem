## Title
Artifact Display

## Slug
artifact-display

## Difficulty
Medium

## Description
Curators remove artifacts from a display row.

The game involves artifacts numbered $1, 2, \dots, n$.
The game is played in turns, and Curator A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining artifacts.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left piece or the right piece from the sequence. The game then continues with the other player.

Both Curator A and Curator B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of artifacts $n$.

## Examples

### 1

#### Input
1

#### Output
Curator A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Curator A removes 1. The remaining sequence is empty (XOR sum 0). Curator B cannot move and loses. Curator A wins.

### 2

#### Input
2

#### Output
Curator B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Curator A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Curator B will then remove the last number, leaving an empty sequence (XOR 0), causing Curator A to lose on the next turn. Curator B wins.

## Input Format
- The only input line has an integer n, the number of artifacts.

## Output Format
- Return "Curator A" if Curator A wins, or "Curator B" if Curator B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
