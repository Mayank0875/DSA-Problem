## Title
Airport Gates

## Slug
airport-gates

## Difficulty
Hard

## Description
Controllers park planes. Taxiways lead to specific gates.

Controller and Weather are playing a strategic game using a gate map $p$ of length $n$. The game starts with a efficiency of 0.

The players take turns, with Controller moving first. On each turn, a player chooses an integer $x$ from the gate map that has not been chosen before.
- If it is Controller's turn, the chosen value $x$ is **added** to the efficiency.
- If it is Weather's turn, the chosen value $x$ is **subtracted** from the efficiency.

The rules for choosing $x$ are:
1. On the very first move of the game, Controller may choose **any** unselected gate from the gate map.
2. On every move after the first:
   - Let $m$ be the index of the gate chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected gate.

The game continues until all gates of the gate map have been chosen.

Controller plays optimally to **maximize** the final efficiency, while Weather plays optimally to **minimize** it.

Your task is to compute the final efficiency assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final efficiency is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final efficiency is 1.

## Input Format
- The first line contains an integer $n$ (length of gate map).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final efficiency on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
