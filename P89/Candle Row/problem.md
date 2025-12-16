## Title
Candle Row

## Slug
candle-row

## Difficulty
Medium

## Description
Monks extinguish candles in a row.

The game involves candles numbered $1, 2, \dots, n$.
The game is played in turns, and Monk 1 always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining candles.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the left candle or the right candle from the sequence. The game then continues with the other player.

Both Monk 1 and Monk 2 are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of candles $n$.

## Examples

### 1

#### Input
1

#### Output
Monk 1

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Monk 1 removes 1. The remaining sequence is empty (XOR sum 0). Monk 2 cannot move and loses. Monk 1 wins.

### 2

#### Input
2

#### Output
Monk 2

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Monk 1 can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Monk 2 will then remove the last number, leaving an empty sequence (XOR 0), causing Monk 1 to lose on the next turn. Monk 2 wins.

## Input Format
- The only input line has an integer n, the number of candles.

## Output Format
- Return "Monk 1" if Monk 1 wins, or "Monk 2" if Monk 2 wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
