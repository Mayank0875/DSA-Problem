## Title
Ant Colony Path

## Slug
ant-colony-path

## Difficulty
Hard

## Description
Ants claim food nodes. Pheromone trails lead to the next specific node.

Red Ants and Black Ants are playing a strategic game using a node map $p$ of length $n$. The game starts with a food gathered of 0.

The players take turns, with Red Ants moving first. On each turn, a player chooses an integer $x$ from the node map that has not been chosen before.
- If it is Red Ants's turn, the chosen value $x$ is **added** to the food gathered.
- If it is Black Ants's turn, the chosen value $x$ is **subtracted** from the food gathered.

The rules for choosing $x$ are:
1. On the very first move of the game, Red Ants may choose **any** unselected node from the node map.
2. On every move after the first:
   - Let $m$ be the index of the node chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected node.

The game continues until all nodes of the node map have been chosen.

Red Ants plays optimally to **maximize** the final food gathered, while Black Ants plays optimally to **minimize** it.

Your task is to compute the final food gathered assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final food gathered is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final food gathered is 1.

## Input Format
- The first line contains an integer $n$ (length of node map).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final food gathered on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
