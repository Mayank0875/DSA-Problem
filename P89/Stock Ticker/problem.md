## Title
Stock Ticker

## Slug
stock-ticker

## Difficulty
Medium

## Description
Traders remove ticker symbols from a screen.

The game involves symbols numbered $1, 2, \dots, n$.
The game is played in turns, and Bull always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining symbols.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the start symbol or the end symbol from the sequence. The game then continues with the other player.

Both Bull and Bear are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of symbols $n$.

## Examples

### 1

#### Input
1

#### Output
Bull

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Bull removes 1. The remaining sequence is empty (XOR sum 0). Bear cannot move and loses. Bull wins.

### 2

#### Input
2

#### Output
Bear

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Bull can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Bear will then remove the last number, leaving an empty sequence (XOR 0), causing Bull to lose on the next turn. Bear wins.

## Input Format
- The only input line has an integer n, the number of symbols.

## Output Format
- Return "Bull" if Bull wins, or "Bear" if Bear wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
