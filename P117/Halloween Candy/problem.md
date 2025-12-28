## Title
Halloween Candy

## Slug
halloween-candy

## Difficulty
Medium

## Description
Siblings trade candy. The Big Brother takes the full-sized bars, the Middle Sibling (you) takes the fun-sized, and the Baby gets the raisins.

There are $3n$ treats of varying sugar content available. The distribution follows a strict protocol. In each round, you must select any 3 treats. The parties then claim them based on the following rules:

1. The **Big Brother** takes the treat with the **maximum** sugar content from the triplet.
2. You, the **Middle Sibling**, take the treat with the **second maximum** sugar content.
3. The **Baby** takes the remaining treat (the one with the minimum sugar content).

This process repeats until all treats are distributed. Your goal as the Middle Sibling is to maximize the total sugar content of the treats you acquire.

Given an array of integers `treats`, where `treats[i]` represents the sugar content of the $i$-th treat, return the maximum total sugar content you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 treats. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Big Brother takes `8`, you take `7`, Baby takes `2`.
2. Pick the remaining `(1, 2, 4)`. Big Brother takes `4`, you take `2`, Baby takes `1`.
Total sugar content = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Big Brother takes `5`, you take `4`, Baby takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of treats.
- The second line contains $3n$ space-separated integers representing the `treats` array.

## Output Format
- Return a single integer representing the maximum total sugar content you can collect.

## Constraints
- 1 ≤ treats.length ≤ 10^5
- `treats.length` is divisible by 3.
- 1 ≤ treats[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
