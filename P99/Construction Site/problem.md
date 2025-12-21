## Title
Construction Site

## Slug
construction-site

## Difficulty
Hard

## Description
Workers lay bricks. The pattern dictates the next brick position.

Mason and Inspector are playing a strategic game using a blueprint $p$ of length $n$. The game starts with a progress of 0.

The players take turns, with Mason moving first. On each turn, a player chooses an integer $x$ from the blueprint that has not been chosen before.
- If it is Mason's turn, the chosen value $x$ is **added** to the progress.
- If it is Inspector's turn, the chosen value $x$ is **subtracted** from the progress.

The rules for choosing $x$ are:
1. On the very first move of the game, Mason may choose **any** unselected brick from the blueprint.
2. On every move after the first:
   - Let $m$ be the index of the brick chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected brick.

The game continues until all bricks of the blueprint have been chosen.

Mason plays optimally to **maximize** the final progress, while Inspector plays optimally to **minimize** it.

Your task is to compute the final progress assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final progress is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final progress is 1.

## Input Format
- The first line contains an integer $n$ (length of blueprint).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final progress on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
