## Title
Software Features

## Slug
software-features

## Difficulty
Medium

## Description
Features are assigned to tiers. Premium gets the AI tools, Standard (you) gets the analytics, and Basic gets the login screen.

There are $3n$ features of varying complexity available. The distribution follows a strict protocol. In each round, you must select any 3 features. The parties then claim them based on the following rules:

1. The **Premium** takes the feature with the **maximum** complexity from the triplet.
2. You, the **Standard**, take the feature with the **second maximum** complexity.
3. The **Basic** takes the remaining feature (the one with the minimum complexity).

This process repeats until all features are distributed. Your goal as the Standard is to maximize the total complexity of the features you acquire.

Given an array of integers `features`, where `features[i]` represents the complexity of the $i$-th feature, return the maximum total complexity you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 features. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Premium takes `8`, you take `7`, Basic takes `2`.
2. Pick the remaining `(1, 2, 4)`. Premium takes `4`, you take `2`, Basic takes `1`.
Total complexity = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Premium takes `5`, you take `4`, Basic takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of features.
- The second line contains $3n$ space-separated integers representing the `features` array.

## Output Format
- Return a single integer representing the maximum total complexity you can collect.

## Constraints
- 1 ≤ features.length ≤ 10^5
- `features.length` is divisible by 3.
- 1 ≤ features[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
