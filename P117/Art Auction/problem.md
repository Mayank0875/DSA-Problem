## Title
Art Auction

## Slug
art-auction

## Difficulty
Medium

## Description
Artworks are sold in lots. The National Museum bids highest, the Private Collector (you) is second, and the Thrift Store buys the rest.

There are $3n$ paintings of varying estimated worth available. The distribution follows a strict protocol. In each round, you must select any 3 paintings. The parties then claim them based on the following rules:

1. The **Museum** takes the painting with the **maximum** estimated worth from the triplet.
2. You, the **Collector**, take the painting with the **second maximum** estimated worth.
3. The **Thrift Store** takes the remaining painting (the one with the minimum estimated worth).

This process repeats until all paintings are distributed. Your goal as the Collector is to maximize the total estimated worth of the paintings you acquire.

Given an array of integers `paintings`, where `paintings[i]` represents the estimated worth of the $i$-th painting, return the maximum total estimated worth you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 paintings. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Museum takes `8`, you take `7`, Thrift Store takes `2`.
2. Pick the remaining `(1, 2, 4)`. Museum takes `4`, you take `2`, Thrift Store takes `1`.
Total estimated worth = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Museum takes `5`, you take `4`, Thrift Store takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of paintings.
- The second line contains $3n$ space-separated integers representing the `paintings` array.

## Output Format
- Return a single integer representing the maximum total estimated worth you can collect.

## Constraints
- 1 ≤ paintings.length ≤ 10^5
- `paintings.length` is divisible by 3.
- 1 ≤ paintings[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
