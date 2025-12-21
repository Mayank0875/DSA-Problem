## Title
Basketball Plays

## Slug
basketball-plays

## Difficulty
Hard

## Description
Coaches call plays. A pass goes to a specific designated player.

Coach and Defense are playing a strategic game using a playbook $p$ of length $n$. The game starts with a points of 0.

The players take turns, with Coach moving first. On each turn, a player chooses an integer $x$ from the playbook that has not been chosen before.
- If it is Coach's turn, the chosen value $x$ is **added** to the points.
- If it is Defense's turn, the chosen value $x$ is **subtracted** from the points.

The rules for choosing $x$ are:
1. On the very first move of the game, Coach may choose **any** unselected player from the playbook.
2. On every move after the first:
   - Let $m$ be the index of the player chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected player.

The game continues until all players of the playbook have been chosen.

Coach plays optimally to **maximize** the final points, while Defense plays optimally to **minimize** it.

Your task is to compute the final points assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final points is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final points is 1.

## Input Format
- The first line contains an integer $n$ (length of playbook).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final points on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
