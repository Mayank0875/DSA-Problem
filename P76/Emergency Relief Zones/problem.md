## Title
Emergency Relief Zones

## Slug
emergency-relief-zones

## Difficulty
Hard

## Description
Relief supplies are dropped to `n` villages along a road by `k` airplanes. Each plane covers a contiguous range of villages. The 'logistical variance' for a plane is the square of the total population it serves.

You must partition the sequence of villages into exactly `k` non-empty contiguous zones.
Each zone corresponds to a airplane.
The "logistical variance" for a airplane is calculated as the **square of the sum** of the populations of the villages in that zone.

Your goal is to minimize the total logistical variance (the sum of the logistical variance values of all `k` zones).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the villages into 3 zones: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total logistical variance is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 zone is allowed, containing all villages. Sum = 15. logistical variance = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of villages and the required number of zones.
- The second line contains `n` integers representing the populations of each village.

## Output Format
- Return one integer: the minimum total logistical variance.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
