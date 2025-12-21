## Title
Ecological Balance

## Slug
ecological-balance

## Difficulty
Hard

## Description
Biologists introduce species. Food chains dictate the next affected species.

Nature and Pollution are playing a strategic game using a species list $p$ of length $n$. The game starts with a biodiversity of 0.

The players take turns, with Nature moving first. On each turn, a player chooses an integer $x$ from the species list that has not been chosen before.
- If it is Nature's turn, the chosen value $x$ is **added** to the biodiversity.
- If it is Pollution's turn, the chosen value $x$ is **subtracted** from the biodiversity.

The rules for choosing $x$ are:
1. On the very first move of the game, Nature may choose **any** unselected species from the species list.
2. On every move after the first:
   - Let $m$ be the index of the species chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected species.

The game continues until all specieses of the species list have been chosen.

Nature plays optimally to **maximize** the final biodiversity, while Pollution plays optimally to **minimize** it.

Your task is to compute the final biodiversity assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final biodiversity is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final biodiversity is 1.

## Input Format
- The first line contains an integer $n$ (length of species list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final biodiversity on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
