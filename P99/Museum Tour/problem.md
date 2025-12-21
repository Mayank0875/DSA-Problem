## Title
Museum Tour

## Slug
museum-tour

## Difficulty
Hard

## Description
Guides show exhibits. The layout leads naturally to the next exhibit.

Guide and Tourist are playing a strategic game using a exhibit list $p$ of length $n$. The game starts with a interest of 0.

The players take turns, with Guide moving first. On each turn, a player chooses an integer $x$ from the exhibit list that has not been chosen before.
- If it is Guide's turn, the chosen value $x$ is **added** to the interest.
- If it is Tourist's turn, the chosen value $x$ is **subtracted** from the interest.

The rules for choosing $x$ are:
1. On the very first move of the game, Guide may choose **any** unselected exhibit from the exhibit list.
2. On every move after the first:
   - Let $m$ be the index of the exhibit chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected exhibit.

The game continues until all exhibits of the exhibit list have been chosen.

Guide plays optimally to **maximize** the final interest, while Tourist plays optimally to **minimize** it.

Your task is to compute the final interest assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final interest is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final interest is 1.

## Input Format
- The first line contains an integer $n$ (length of exhibit list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final interest on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
