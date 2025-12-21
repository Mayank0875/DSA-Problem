## Title
Satellite Link

## Slug
satellite-link

## Difficulty
Hard

## Description
Operators uplink to satellites. Satellites relay signal to a fixed peer.

Operator and Jammer are playing a strategic game using a constellation $p$ of length $n$. The game starts with a uptime of 0.

The players take turns, with Operator moving first. On each turn, a player chooses an integer $x$ from the constellation that has not been chosen before.
- If it is Operator's turn, the chosen value $x$ is **added** to the uptime.
- If it is Jammer's turn, the chosen value $x$ is **subtracted** from the uptime.

The rules for choosing $x$ are:
1. On the very first move of the game, Operator may choose **any** unselected satellite from the constellation.
2. On every move after the first:
   - Let $m$ be the index of the satellite chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected satellite.

The game continues until all satellites of the constellation have been chosen.

Operator plays optimally to **maximize** the final uptime, while Jammer plays optimally to **minimize** it.

Your task is to compute the final uptime assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final uptime is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final uptime is 1.

## Input Format
- The first line contains an integer $n$ (length of constellation).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final uptime on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
