## Title
Library Bookshelf

## Slug
library-bookshelf

## Difficulty
Medium

## Description
Librarians remove books from a shelf to solve a puzzle.

The game involves books numbered $1, 2, \dots, n$.
The game is played in turns, and Bookworm always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining books.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the first book or the last book from the sequence. The game then continues with the other player.

Both Bookworm and Scholar are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of books $n$.

## Examples

### 1

#### Input
1

#### Output
Bookworm

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Bookworm removes 1. The remaining sequence is empty (XOR sum 0). Scholar cannot move and loses. Bookworm wins.

### 2

#### Input
2

#### Output
Scholar

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Bookworm can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Scholar will then remove the last number, leaving an empty sequence (XOR 0), causing Bookworm to lose on the next turn. Scholar wins.

## Input Format
- The only input line has an integer n, the number of books.

## Output Format
- Return "Bookworm" if Bookworm wins, or "Scholar" if Scholar wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
