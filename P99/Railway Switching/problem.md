## Title
Railway Switching

## Slug
railway-switching

## Difficulty
Hard

## Description
Controllers switch tracks. Tracks lead physically to specific next junctions.

Controller and Saboteur are playing a strategic game using a track layout $p$ of length $n$. The game starts with a throughput of 0.

The players take turns, with Controller moving first. On each turn, a player chooses an integer $x$ from the track layout that has not been chosen before.
- If it is Controller's turn, the chosen value $x$ is **added** to the throughput.
- If it is Saboteur's turn, the chosen value $x$ is **subtracted** from the throughput.

The rules for choosing $x$ are:
1. On the very first move of the game, Controller may choose **any** unselected junction from the track layout.
2. On every move after the first:
   - Let $m$ be the index of the junction chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected junction.

The game continues until all junctions of the track layout have been chosen.

Controller plays optimally to **maximize** the final throughput, while Saboteur plays optimally to **minimize** it.

Your task is to compute the final throughput assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final throughput is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final throughput is 1.

## Input Format
- The first line contains an integer $n$ (length of track layout).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final throughput on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
