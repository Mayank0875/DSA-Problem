## Title
Fishing Catch

## Slug
fishing-catch

## Difficulty
Medium

## Description
Fish are sold at the dock. The Market buys the prize tuna, the Restaurant (you) buys the salmon, and the Bait Shop buys the minnows.

There are $3n$ fish of varying weight available. The distribution follows a strict protocol. In each round, you must select any 3 fish. The parties then claim them based on the following rules:

1. The **Market** takes the fish with the **maximum** weight from the triplet.
2. You, the **Restaurant**, take the fish with the **second maximum** weight.
3. The **Bait Shop** takes the remaining fish (the one with the minimum weight).

This process repeats until all fish are distributed. Your goal as the Restaurant is to maximize the total weight of the fish you acquire.

Given an array of integers `fish`, where `fish[i]` represents the weight of the $i$-th fish, return the maximum total weight you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 fish. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Market takes `8`, you take `7`, Bait Shop takes `2`.
2. Pick the remaining `(1, 2, 4)`. Market takes `4`, you take `2`, Bait Shop takes `1`.
Total weight = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Market takes `5`, you take `4`, Bait Shop takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of fish.
- The second line contains $3n$ space-separated integers representing the `fish` array.

## Output Format
- Return a single integer representing the maximum total weight you can collect.

## Constraints
- 1 ≤ fish.length ≤ 10^5
- `fish.length` is divisible by 3.
- 1 ≤ fish[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
