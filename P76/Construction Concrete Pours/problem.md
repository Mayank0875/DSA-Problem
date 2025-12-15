## Title
Construction Concrete Pours

## Slug
construction-concrete-pours

## Difficulty
Hard

## Description
A construction crew pours a sidewalk in `n` sections using `k` truckloads of concrete. Each section requires a specific volume. A truck serves a contiguous range of sections. The 'wear' on a truck is the square of the total volume it delivers.

You must partition the sequence of sections into exactly `k` non-empty contiguous deliveries.
Each delivery corresponds to a truck.
The "wear" for a truck is calculated as the **square of the sum** of the volumes of the sections in that delivery.

Your goal is to minimize the total wear (the sum of the wear values of all `k` deliveries).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the sections into 3 deliveries: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total wear is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 delivery is allowed, containing all sections. Sum = 15. wear = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of sections and the required number of deliveries.
- The second line contains `n` integers representing the volumes of each section.

## Output Format
- Return one integer: the minimum total wear.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
