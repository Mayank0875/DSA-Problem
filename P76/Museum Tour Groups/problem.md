## Title
Museum Tour Groups

## Slug
museum-tour-groups

## Difficulty
Hard

## Description
A museum queue has `n` visitors with different group sizes. They are split into `k` guided tours. Visitors stay in queue order. The 'noise level' of a tour is the square of the total number of people in it.

You must partition the sequence of visitor groups into exactly `k` non-empty contiguous tours.
Each tour corresponds to a guide.
The "noise level" for a guide is calculated as the **square of the sum** of the counts of the visitor groups in that tour.

Your goal is to minimize the total noise level (the sum of the noise level values of all `k` tours).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the visitor groups into 3 tours: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total noise level is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 tour is allowed, containing all visitor groups. Sum = 15. noise level = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of visitor groups and the required number of tours.
- The second line contains `n` integers representing the counts of each group.

## Output Format
- Return one integer: the minimum total noise level.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
