## Title
Music Playlist

## Slug
music-playlist

## Difficulty
Hard

## Description
DJs pick songs. Songs crossfade into specific next tracks.

DJ A and DJ B are playing a strategic game using a playlist $p$ of length $n$. The game starts with a crowd energy of 0.

The players take turns, with DJ A moving first. On each turn, a player chooses an integer $x$ from the playlist that has not been chosen before.
- If it is DJ A's turn, the chosen value $x$ is **added** to the crowd energy.
- If it is DJ B's turn, the chosen value $x$ is **subtracted** from the crowd energy.

The rules for choosing $x$ are:
1. On the very first move of the game, DJ A may choose **any** unselected song from the playlist.
2. On every move after the first:
   - Let $m$ be the index of the song chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected song.

The game continues until all songs of the playlist have been chosen.

DJ A plays optimally to **maximize** the final crowd energy, while DJ B plays optimally to **minimize** it.

Your task is to compute the final crowd energy assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final crowd energy is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final crowd energy is 1.

## Input Format
- The first line contains an integer $n$ (length of playlist).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final crowd energy on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
