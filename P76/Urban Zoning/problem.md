## Title
Urban Zoning

## Slug
urban-zoning

## Difficulty
Hard

## Description
A city street has `n` blocks with different population densities. Planners divide the street into `k` zones. The 'infrastructure load' of a zone is the square of the total population in that zone.

You must partition the sequence of blocks into exactly `k` non-empty contiguous zones.
Each zone corresponds to a zone.
The "infrastructure load" for a zone is calculated as the **square of the sum** of the populations of the blocks in that zone.

Your goal is to minimize the total infrastructure load (the sum of the infrastructure load values of all `k` zones).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the blocks into 3 zones: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total infrastructure load is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 zone is allowed, containing all blocks. Sum = 15. infrastructure load = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of blocks and the required number of zones.
- The second line contains `n` integers representing the populations of each block.

## Output Format
- Return one integer: the minimum total infrastructure load.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
