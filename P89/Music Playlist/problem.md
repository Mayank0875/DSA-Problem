## Title
Music Playlist

## Slug
music-playlist

## Difficulty
Medium

## Description
DJs remove songs from a playlist queue.

The game involves songs numbered $1, 2, \dots, n$.
The game is played in turns, and DJ Alpha always goes first. On a player's turn, they must check the bitwise XOR sum of the numbers on all remaining songs.
* If the XOR sum is **0**, the current player cannot make a move and immediately **loses** the game.
* If the XOR sum is **not 0**, the player must remove either the top song or the bottom song from the sequence. The game then continues with the other player.

Both DJ Alpha and DJ Beta are highly intelligent and play optimally to win. Your task is to determine who will win the game for a given number of songs $n$.

## Examples

### 1

#### Input
1

#### Output
DJ Alpha

#### Explanation
The sequence is [1]. XOR sum is 1 != 0. DJ Alpha removes 1. The remaining sequence is empty (XOR sum 0). DJ Beta cannot move and loses. DJ Alpha wins.

### 2

#### Input
2

#### Output
DJ Beta

#### Explanation
The sequence is [1, 2]. XOR sum is 3. DJ Alpha can remove 1 (leaving [2], XOR 2) or 2 (leaving [1], XOR 1). In either case, the remaining XOR is non-zero. DJ Beta will then remove the last number, leaving an empty sequence (XOR 0), causing DJ Alpha to lose on the next turn. DJ Beta wins.

## Input Format
- The only input line has an integer n, the number of songs.

## Output Format
- Return "DJ Alpha" if DJ Alpha wins, or "DJ Beta" if DJ Beta wins.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths
