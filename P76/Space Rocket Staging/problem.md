## Title
Space Rocket Staging

## Slug
space-rocket-staging

## Difficulty
Hard

## Description
A rocket mission has `n` maneuvers to perform using `k` fuel stages. Each maneuver requires specific Delta-V. Maneuvers are performed sequentially. The 'structural stress' on a stage is the square of the total Delta-V it provides.

You must partition the sequence of maneuvers into exactly `k` non-empty contiguous sets.
Each set corresponds to a stage.
The "structural stress" for a stage is calculated as the **square of the sum** of the Delta-V requirements of the maneuvers in that set.

Your goal is to minimize the total structural stress (the sum of the structural stress values of all `k` sets).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the maneuvers into 3 sets: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total structural stress is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 set is allowed, containing all maneuvers. Sum = 15. structural stress = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of maneuvers and the required number of sets.
- The second line contains `n` integers representing the Delta-V requirements of each maneuver.

## Output Format
- Return one integer: the minimum total structural stress.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
