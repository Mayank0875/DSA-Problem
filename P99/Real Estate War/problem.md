## Title
Real Estate War

## Slug
real-estate-war

## Difficulty
Hard

## Description
Tycoons buy properties. Deeds contain clauses mandating the next purchase.

Tycoon A and Tycoon B are playing a strategic game using a property listings $p$ of length $n$. The game starts with a net worth of 0.

The players take turns, with Tycoon A moving first. On each turn, a player chooses an integer $x$ from the property listings that has not been chosen before.
- If it is Tycoon A's turn, the chosen value $x$ is **added** to the net worth.
- If it is Tycoon B's turn, the chosen value $x$ is **subtracted** from the net worth.

The rules for choosing $x$ are:
1. On the very first move of the game, Tycoon A may choose **any** unselected property from the property listings.
2. On every move after the first:
   - Let $m$ be the index of the property chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected property.

The game continues until all properties of the property listings have been chosen.

Tycoon A plays optimally to **maximize** the final net worth, while Tycoon B plays optimally to **minimize** it.

Your task is to compute the final net worth assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final net worth is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final net worth is 1.

## Input Format
- The first line contains an integer $n$ (length of property listings).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final net worth on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
