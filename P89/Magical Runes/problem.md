## Title
Magical Runes

## Slug
magical-runes

## Difficulty
Medium

## Description
Two wizards duel using a line of magical runes.

The game involves runes numbered $1, 2, \dots, n$.
The game is played in turns, and Wizard A always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining runes.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the leftmost rune or the rightmost rune from the sequence. The game then continues with the other player.

Both Wizard A and Wizard B are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of runes $n$.

## Examples

### 1

#### Input
1

#### Output
Wizard A

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Wizard A removes 1. The remaining sequence is empty (XOR sum 0). Wizard B cannot move and loses. Wizard A wins.

### 2

#### Input
2

#### Output
Wizard B

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Wizard A can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Wizard B will then remove the last number, leaving an empty sequence (XOR 0), causing Wizard A to lose on the next turn. Wizard B wins.

## Input Format
- The only input line has an integer n, the number of runes.

## Output Format
- Return "Wizard A" if Wizard A wins, or "Wizard B" if Wizard B wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
