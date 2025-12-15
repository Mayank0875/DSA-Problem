## Title
Snow Plowing Route

## Slug
snow-plowing-route

## Difficulty
Hard

## Description
A highway has `n` segments with varying snow depth. `k` snowplows are deployed to clear contiguous sections. The 'fuel consumption rate' for a plow is the square of the total snow mass it clears.

You must partition the sequence of segments into exactly `k` non-empty contiguous assignments.
Each assignment corresponds to a plow.
The "fuel consumption rate" for a plow is calculated as the **square of the sum** of the snow masses of the segments in that assignment.

Your goal is to minimize the total fuel consumption rate (the sum of the fuel consumption rate values of all `k` assignments).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the segments into 3 assignments: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total fuel consumption rate is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 assignment is allowed, containing all segments. Sum = 15. fuel consumption rate = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of segments and the required number of assignments.
- The second line contains `n` integers representing the snow masses of each segment.

## Output Format
- Return one integer: the minimum total fuel consumption rate.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
