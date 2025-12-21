## Title
Glacier Melting

## Slug
glacier-melting

## Difficulty
Hard

## Description
Scientists track cracks. A fissure propagates to a specific weak point.

Scientist and Heat are playing a strategic game using a ice sheet $p$ of length $n$. The game starts with a stability of 0.

The players take turns, with Scientist moving first. On each turn, a player chooses an integer $x$ from the ice sheet that has not been chosen before.
- If it is Scientist's turn, the chosen value $x$ is **added** to the stability.
- If it is Heat's turn, the chosen value $x$ is **subtracted** from the stability.

The rules for choosing $x$ are:
1. On the very first move of the game, Scientist may choose **any** unselected crack from the ice sheet.
2. On every move after the first:
   - Let $m$ be the index of the crack chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected crack.

The game continues until all cracks of the ice sheet have been chosen.

Scientist plays optimally to **maximize** the final stability, while Heat plays optimally to **minimize** it.

Your task is to compute the final stability assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final stability is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final stability is 1.

## Input Format
- The first line contains an integer $n$ (length of ice sheet).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final stability on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
