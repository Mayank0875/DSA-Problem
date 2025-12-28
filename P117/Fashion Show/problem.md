## Title
Fashion Show

## Slug
fashion-show

## Difficulty
Medium

## Description
Clothes are distributed. The Runway gets the couture, the Boutique (you) gets the ready-to-wear, and the Outlet gets last season.

There are $3n$ garments of varying style score available. The distribution follows a strict protocol. In each round, you must select any 3 garments. The parties then claim them based on the following rules:

1. The **Runway** takes the garment with the **maximum** style score from the triplet.
2. You, the **Boutique**, take the garment with the **second maximum** style score.
3. The **Outlet** takes the remaining garment (the one with the minimum style score).

This process repeats until all garments are distributed. Your goal as the Boutique is to maximize the total style score of the garments you acquire.

Given an array of integers `garments`, where `garments[i]` represents the style score of the $i$-th garment, return the maximum total style score you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 garments. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Runway takes `8`, you take `7`, Outlet takes `2`.
2. Pick the remaining `(1, 2, 4)`. Runway takes `4`, you take `2`, Outlet takes `1`.
Total style score = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Runway takes `5`, you take `4`, Outlet takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of garments.
- The second line contains $3n$ space-separated integers representing the `garments` array.

## Output Format
- Return a single integer representing the maximum total style score you can collect.

## Constraints
- 1 ≤ garments.length ≤ 10^5
- `garments.length` is divisible by 3.
- 1 ≤ garments[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
