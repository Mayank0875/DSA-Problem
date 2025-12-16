## Title
Card Removal Game

## Slug
card-removal-game

## Difficulty
Medium

## Description
Players remove cards from a row to force the opponent into a void state.

The game involves cards numbered $1, 2, \dots, n$.
The game is played in turns, and Alice always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining cards.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left card or the right card from the sequence. The game then continues with the other player.

Both Alice and Bob are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of cards $n$.

## Examples

### 1

#### Input
1

#### Output
Alice

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Alice removes 1. The remaining sequence is empty (XOR sum 0). Bob cannot move and loses. Alice wins.

### 2

#### Input
2

#### Output
Bob

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Alice can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Bob will then remove the last number, leaving an empty sequence (XOR 0), causing Alice to lose on the next turn. Bob wins.

## Input Format
- The only input line has an integer n, the number of cards.

## Output Format
- Return "Alice" if Alice wins, or "Bob" if Bob wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
