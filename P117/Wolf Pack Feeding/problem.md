## Title
Wolf Pack Feeding

## Slug
wolf-pack-feeding

## Difficulty
Medium

## Description
A pack of wolves divides the hunt. The Alpha eats first, the Beta (you) eats second, and the Omega eats scraps.

There are $3n$ meat chunks of varying weight available. The distribution follows a strict protocol. In each round, you must select any 3 meat chunks. The parties then claim them based on the following rules:

1. The **Alpha** takes the chunk with the **maximum** weight from the triplet.
2. You, the **Beta**, take the chunk with the **second maximum** weight.
3. The **Omega** takes the remaining chunk (the one with the minimum weight).

This process repeats until all meat chunks are distributed. Your goal as the Beta is to maximize the total weight of the meat chunks you acquire.

Given an array of integers `chunks`, where `chunks[i]` represents the weight of the $i$-th chunk, return the maximum total weight you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 meat chunks. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Alpha takes `8`, you take `7`, Omega takes `2`.
2. Pick the remaining `(1, 2, 4)`. Alpha takes `4`, you take `2`, Omega takes `1`.
Total weight = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Alpha takes `5`, you take `4`, Omega takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of meat chunks.
- The second line contains $3n$ space-separated integers representing the `chunks` array.

## Output Format
- Return a single integer representing the maximum total weight you can collect.

## Constraints
- 1 ≤ chunks.length ≤ 10^5
- `chunks.length` is divisible by 3.
- 1 ≤ chunks[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
