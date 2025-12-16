## Title
Digital Data Stream

## Slug
digital-data-stream

## Difficulty
Medium

## Description
Two hackers compete to crash a system by manipulating a data stream.

The game involves data packets numbered $1, 2, \dots, n$.
The game is played in turns, and Hacker Red always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining data packets.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the first packet or the last packet from the sequence. The game then continues with the other player.

Both Hacker Red and Hacker Blue are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of data packets $n$.

## Examples

### 1

#### Input
1

#### Output
Hacker Red

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. Hacker Red removes 1. The remaining sequence is empty (XOR sum 0). Hacker Blue cannot move and loses. Hacker Red wins.

### 2

#### Input
2

#### Output
Hacker Blue

#### Explanation
The sequence is [1, 2]. XOR sum is 3. Hacker Red can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. Hacker Blue will then remove the last number, leaving an empty sequence (XOR 0), causing Hacker Red to lose on the next turn. Hacker Blue wins.

## Input Format
- The only input line has an integer n, the number of data packets.

## Output Format
- Return "Hacker Red" if Hacker Red wins, or "Hacker Blue" if Hacker Blue wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
