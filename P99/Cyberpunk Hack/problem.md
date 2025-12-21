## Title
Cyberpunk Hack

## Slug
cyberpunk-hack

## Difficulty
Hard

## Description
Hackers capture nodes in a network. Capturing a node reveals the next target.

Neo and Smith are playing a strategic game using a node array $p$ of length $n$. The game starts with a system integrity of 0.

The players take turns, with Neo moving first. On each turn, a player chooses an integer $x$ from the node array that has not been chosen before.
- If it is Neo's turn, the chosen value $x$ is **added** to the system integrity.
- If it is Smith's turn, the chosen value $x$ is **subtracted** from the system integrity.

The rules for choosing $x$ are:
1. On the very first move of the game, Neo may choose **any** unselected node from the node array.
2. On every move after the first:
   - Let $m$ be the index of the node chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected node.

The game continues until all nodes of the node array have been chosen.

Neo plays optimally to **maximize** the final system integrity, while Smith plays optimally to **minimize** it.

Your task is to compute the final system integrity assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final system integrity is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final system integrity is 1.

## Input Format
- The first line contains an integer $n$ (length of node array).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final system integrity on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
