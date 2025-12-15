## Title
Welding Pipeline Seams

## Slug
welding-pipeline-seams

## Difficulty
Hard

## Description
A pipeline has `n` segments. `k` welding robots join contiguous segments. The 'energy consumption' for a robot is the square of the total length of segments it welds.

You must partition the sequence of segments into exactly `k` non-empty contiguous assignments.
Each assignment corresponds to a robot.
The "energy consumption" for a robot is calculated as the **square of the sum** of the lengths of the segments in that assignment.

Your goal is to minimize the total energy consumption (the sum of the energy consumption values of all `k` assignments).

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
The total energy consumption is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 assignment is allowed, containing all segments. Sum = 15. energy consumption = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of segments and the required number of assignments.
- The second line contains `n` integers representing the lengths of each segment.

## Output Format
- Return one integer: the minimum total energy consumption.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
