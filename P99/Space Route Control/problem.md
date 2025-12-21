## Title
Space Route Control

## Slug
space-route-control

## Difficulty
Hard

## Description
Two space admirals fight for control of jump gates.

Admiral Vance and Commander Zorg are playing a strategic game using a gate permutation $p$ of length $n$. The game starts with a control score of 0.

The players take turns, with Admiral Vance moving first. On each turn, a player chooses an integer $x$ from the gate permutation that has not been chosen before.
- If it is Admiral Vance's turn, the chosen value $x$ is **added** to the control score.
- If it is Commander Zorg's turn, the chosen value $x$ is **subtracted** from the control score.

The rules for choosing $x$ are:
1. On the very first move of the game, Admiral Vance may choose **any** unselected gate from the gate permutation.
2. On every move after the first:
   - Let $m$ be the index of the gate chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected gate.

The game continues until all gates of the gate permutation have been chosen.

Admiral Vance plays optimally to **maximize** the final control score, while Commander Zorg plays optimally to **minimize** it.

Your task is to compute the final control score assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final control score is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final control score is 1.

## Input Format
- The first line contains an integer $n$ (length of gate permutation).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final control score on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
