## Title
Zoo Feeding

## Slug
zoo-feeding

## Difficulty
Medium

## Description
Meat is distributed. The Lion gets the prime steak, the Bear (you) gets the salmon, and the Monkey gets the fruit (okay, value is calories).

There are $3n$ meals of varying calories available. The distribution follows a strict protocol. In each round, you must select any 3 meals. The parties then claim them based on the following rules:

1. The **Lion** takes the meal with the **maximum** calories from the triplet.
2. You, the **Bear**, take the meal with the **second maximum** calories.
3. The **Monkey** takes the remaining meal (the one with the minimum calories).

This process repeats until all meals are distributed. Your goal as the Bear is to maximize the total calories of the meals you acquire.

Given an array of integers `meals`, where `meals[i]` represents the calories of the $i$-th meal, return the maximum total calories you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 meals. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Lion takes `8`, you take `7`, Monkey takes `2`.
2. Pick the remaining `(1, 2, 4)`. Lion takes `4`, you take `2`, Monkey takes `1`.
Total calories = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Lion takes `5`, you take `4`, Monkey takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of meals.
- The second line contains $3n$ space-separated integers representing the `meals` array.

## Output Format
- Return a single integer representing the maximum total calories you can collect.

## Constraints
- 1 ≤ meals.length ≤ 10^5
- `meals.length` is divisible by 3.
- 1 ≤ meals[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
