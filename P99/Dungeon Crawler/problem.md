## Title
Dungeon Crawler

## Slug
dungeon-crawler

## Difficulty
Hard

## Description
Adventurers clear rooms. Doors lead to specific next rooms.

Knight and Monster are playing a strategic game using a dungeon map $p$ of length $n$. The game starts with a loot of 0.

The players take turns, with Knight moving first. On each turn, a player chooses an integer $x$ from the dungeon map that has not been chosen before.
- If it is Knight's turn, the chosen value $x$ is **added** to the loot.
- If it is Monster's turn, the chosen value $x$ is **subtracted** from the loot.

The rules for choosing $x$ are:
1. On the very first move of the game, Knight may choose **any** unselected room from the dungeon map.
2. On every move after the first:
   - Let $m$ be the index of the room chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected room.

The game continues until all rooms of the dungeon map have been chosen.

Knight plays optimally to **maximize** the final loot, while Monster plays optimally to **minimize** it.

Your task is to compute the final loot assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final loot is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final loot is 1.

## Input Format
- The first line contains an integer $n$ (length of dungeon map).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final loot on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
