## Title
Pipeline Flow

## Slug
pipeline-flow

## Difficulty
Hard

## Description
Engineers open valves. Pressure forces flow to the next valve.

Engineer and Leak are playing a strategic game using a pipe network $p$ of length $n$. The game starts with a pressure of 0.

The players take turns, with Engineer moving first. On each turn, a player chooses an integer $x$ from the pipe network that has not been chosen before.
- If it is Engineer's turn, the chosen value $x$ is **added** to the pressure.
- If it is Leak's turn, the chosen value $x$ is **subtracted** from the pressure.

The rules for choosing $x$ are:
1. On the very first move of the game, Engineer may choose **any** unselected valve from the pipe network.
2. On every move after the first:
   - Let $m$ be the index of the valve chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected valve.

The game continues until all valves of the pipe network have been chosen.

Engineer plays optimally to **maximize** the final pressure, while Leak plays optimally to **minimize** it.

Your task is to compute the final pressure assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final pressure is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final pressure is 1.

## Input Format
- The first line contains an integer $n$ (length of pipe network).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final pressure on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
