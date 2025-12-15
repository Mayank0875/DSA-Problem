## Title
Waste Management

## Slug
waste-management

## Difficulty
Hard

## Description
Garbage trucks collect from `n` neighborhoods. There are `k` dump sites. Trucks collect contiguous routes before dumping. The 'compactor stress' is the square of the total waste weight in a truckload.

You must partition the sequence of neighborhoods into exactly `k` non-empty contiguous loads.
Each load corresponds to a truck.
The "compactor stress" for a truck is calculated as the **square of the sum** of the waste weights of the neighborhoods in that load.

Your goal is to minimize the total compactor stress (the sum of the compactor stress values of all `k` loads).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the neighborhoods into 3 loads: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total compactor stress is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 load is allowed, containing all neighborhoods. Sum = 15. compactor stress = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of neighborhoods and the required number of loads.
- The second line contains `n` integers representing the waste weights of each neighborhood.

## Output Format
- Return one integer: the minimum total compactor stress.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
