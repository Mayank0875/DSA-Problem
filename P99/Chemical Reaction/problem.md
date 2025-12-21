## Title
Chemical Reaction

## Slug
chemical-reaction

## Difficulty
Hard

## Description
Chemists add reagents. Reactions trigger a specific next reagent requirement.

Chemist X and Chemist Y are playing a strategic game using a reagent chain $p$ of length $n$. The game starts with a yield of 0.

The players take turns, with Chemist X moving first. On each turn, a player chooses an integer $x$ from the reagent chain that has not been chosen before.
- If it is Chemist X's turn, the chosen value $x$ is **added** to the yield.
- If it is Chemist Y's turn, the chosen value $x$ is **subtracted** from the yield.

The rules for choosing $x$ are:
1. On the very first move of the game, Chemist X may choose **any** unselected reagent from the reagent chain.
2. On every move after the first:
   - Let $m$ be the index of the reagent chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected reagent.

The game continues until all reagents of the reagent chain have been chosen.

Chemist X plays optimally to **maximize** the final yield, while Chemist Y plays optimally to **minimize** it.

Your task is to compute the final yield assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final yield is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final yield is 1.

## Input Format
- The first line contains an integer $n$ (length of reagent chain).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final yield on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
