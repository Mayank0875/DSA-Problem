## Title
Logistics Hub Sort

## Slug
logistics-hub-sort

## Difficulty
Hard

## Description
Packages arrive on a belt in `n` groups. They are diverted into `k` chutes. Groups stay together. The 'jamming probability' of a chute is the square of the total package volume directed to it.

You must partition the sequence of groups into exactly `k` non-empty contiguous chutes.
Each chute corresponds to a chute.
The "jamming probability" for a chute is calculated as the **square of the sum** of the volumes of the groups in that chute.

Your goal is to minimize the total jamming probability (the sum of the jamming probability values of all `k` chutes).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the groups into 3 chutes: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total jamming probability is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 chute is allowed, containing all groups. Sum = 15. jamming probability = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of groups and the required number of chutes.
- The second line contains `n` integers representing the volumes of each group.

## Output Format
- Return one integer: the minimum total jamming probability.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
