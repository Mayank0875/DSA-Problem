## Title
Fashion Show

## Slug
fashion-show

## Difficulty
Hard

## Description
Designers send models. The runway order is predetermined.

Designer and Critic are playing a strategic game using a runway list $p$ of length $n$. The game starts with a style score of 0.

The players take turns, with Designer moving first. On each turn, a player chooses an integer $x$ from the runway list that has not been chosen before.
- If it is Designer's turn, the chosen value $x$ is **added** to the style score.
- If it is Critic's turn, the chosen value $x$ is **subtracted** from the style score.

The rules for choosing $x$ are:
1. On the very first move of the game, Designer may choose **any** unselected model from the runway list.
2. On every move after the first:
   - Let $m$ be the index of the model chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected model.

The game continues until all models of the runway list have been chosen.

Designer plays optimally to **maximize** the final style score, while Critic plays optimally to **minimize** it.

Your task is to compute the final style score assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final style score is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final style score is 1.

## Input Format
- The first line contains an integer $n$ (length of runway list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final style score on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
