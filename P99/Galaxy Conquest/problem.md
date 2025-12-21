## Title
Galaxy Conquest

## Slug
galaxy-conquest

## Difficulty
Hard

## Description
Empires claim planets. Hyperlanes connect planets to specific neighbors.

Empire and Rebels are playing a strategic game using a star map $p$ of length $n$. The game starts with a influence of 0.

The players take turns, with Empire moving first. On each turn, a player chooses an integer $x$ from the star map that has not been chosen before.
- If it is Empire's turn, the chosen value $x$ is **added** to the influence.
- If it is Rebels's turn, the chosen value $x$ is **subtracted** from the influence.

The rules for choosing $x$ are:
1. On the very first move of the game, Empire may choose **any** unselected planet from the star map.
2. On every move after the first:
   - Let $m$ be the index of the planet chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected planet.

The game continues until all planets of the star map have been chosen.

Empire plays optimally to **maximize** the final influence, while Rebels plays optimally to **minimize** it.

Your task is to compute the final influence assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final influence is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final influence is 1.

## Input Format
- The first line contains an integer $n$ (length of star map).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final influence on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
