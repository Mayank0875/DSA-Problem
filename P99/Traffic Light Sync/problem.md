## Title
Traffic Light Sync

## Slug
traffic-light-sync

## Difficulty
Hard

## Description
Engineers set green lights. One green light triggers the next intersection.

Engineer and Gridlock are playing a strategic game using a light grid $p$ of length $n$. The game starts with a flow rate of 0.

The players take turns, with Engineer moving first. On each turn, a player chooses an integer $x$ from the light grid that has not been chosen before.
- If it is Engineer's turn, the chosen value $x$ is **added** to the flow rate.
- If it is Gridlock's turn, the chosen value $x$ is **subtracted** from the flow rate.

The rules for choosing $x$ are:
1. On the very first move of the game, Engineer may choose **any** unselected light from the light grid.
2. On every move after the first:
   - Let $m$ be the index of the light chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected light.

The game continues until all lights of the light grid have been chosen.

Engineer plays optimally to **maximize** the final flow rate, while Gridlock plays optimally to **minimize** it.

Your task is to compute the final flow rate assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final flow rate is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final flow rate is 1.

## Input Format
- The first line contains an integer $n$ (length of light grid).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final flow rate on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
