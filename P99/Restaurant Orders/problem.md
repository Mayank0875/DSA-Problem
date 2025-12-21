## Title
Restaurant Orders

## Slug
restaurant-orders

## Difficulty
Hard

## Description
Chefs cook dishes. Recipes require the next ingredient step.

Chef and Waiter are playing a strategic game using a prep list $p$ of length $n$. The game starts with a quality of 0.

The players take turns, with Chef moving first. On each turn, a player chooses an integer $x$ from the prep list that has not been chosen before.
- If it is Chef's turn, the chosen value $x$ is **added** to the quality.
- If it is Waiter's turn, the chosen value $x$ is **subtracted** from the quality.

The rules for choosing $x$ are:
1. On the very first move of the game, Chef may choose **any** unselected ingredient from the prep list.
2. On every move after the first:
   - Let $m$ be the index of the ingredient chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected ingredient.

The game continues until all ingredients of the prep list have been chosen.

Chef plays optimally to **maximize** the final quality, while Waiter plays optimally to **minimize** it.

Your task is to compute the final quality assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final quality is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final quality is 1.

## Input Format
- The first line contains an integer $n$ (length of prep list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final quality on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
