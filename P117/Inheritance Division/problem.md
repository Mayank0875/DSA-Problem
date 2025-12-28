## Title
Inheritance Division

## Slug
inheritance-division

## Difficulty
Medium

## Description
An estate is being divided among three siblings: the Eldest, the Middle Child (you), and the Youngest.

There are $3n$ heirlooms of varying appraised value available. The distribution follows a strict protocol. In each round, you must select any 3 heirlooms. The parties then claim them based on the following rules:

1. The **Eldest** takes the heirloom with the **maximum** appraised value from the triplet.
2. You, the **Middle Child**, take the heirloom with the **second maximum** appraised value.
3. The **Youngest** takes the remaining heirloom (the one with the minimum appraised value).

This process repeats until all heirlooms are distributed. Your goal as the Middle Child is to maximize the total appraised value of the heirlooms you acquire.

Given an array of integers `heirlooms`, where `heirlooms[i]` represents the appraised value of the $i$-th heirloom, return the maximum total appraised value you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 heirlooms. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Eldest takes `8`, you take `7`, Youngest takes `2`.
2. Pick the remaining `(1, 2, 4)`. Eldest takes `4`, you take `2`, Youngest takes `1`.
Total appraised value = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Eldest takes `5`, you take `4`, Youngest takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of heirlooms.
- The second line contains $3n$ space-separated integers representing the `heirlooms` array.

## Output Format
- Return a single integer representing the maximum total appraised value you can collect.

## Constraints
- 1 ≤ heirlooms.length ≤ 10^5
- `heirlooms.length` is divisible by 3.
- 1 ≤ heirlooms[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
