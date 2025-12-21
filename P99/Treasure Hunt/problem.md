## Title
Treasure Hunt

## Slug
treasure-hunt

## Difficulty
Hard

## Description
Pirates pick islands to loot. Maps found on islands point to the next location.

Captain Jack and Barbossa are playing a strategic game using a island map $p$ of length $n$. The game starts with a gold value of 0.

The players take turns, with Captain Jack moving first. On each turn, a player chooses an integer $x$ from the island map that has not been chosen before.
- If it is Captain Jack's turn, the chosen value $x$ is **added** to the gold value.
- If it is Barbossa's turn, the chosen value $x$ is **subtracted** from the gold value.

The rules for choosing $x$ are:
1. On the very first move of the game, Captain Jack may choose **any** unselected island from the island map.
2. On every move after the first:
   - Let $m$ be the index of the island chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected island.

The game continues until all islands of the island map have been chosen.

Captain Jack plays optimally to **maximize** the final gold value, while Barbossa plays optimally to **minimize** it.

Your task is to compute the final gold value assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final gold value is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final gold value is 1.

## Input Format
- The first line contains an integer $n$ (length of island map).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final gold value on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
