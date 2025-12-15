## Title
Irrigation Zones

## Slug
irrigation-zones

## Difficulty
Hard

## Description
A long field with `n` crop rows is watered by `k` sprinklers. Each sprinkler covers a contiguous set of rows. The 'water pressure load' on a sprinkler is the square of the total water demand of the rows it covers.

You must partition the sequence of rows into exactly `k` non-empty contiguous zones.
Each zone corresponds to a sprinkler.
The "water pressure load" for a sprinkler is calculated as the **square of the sum** of the water demands of the rows in that zone.

Your goal is to minimize the total water pressure load (the sum of the water pressure load values of all `k` zones).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the rows into 3 zones: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total water pressure load is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 zone is allowed, containing all rows. Sum = 15. water pressure load = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of rows and the required number of zones.
- The second line contains `n` integers representing the water demands of each row.

## Output Format
- Return one integer: the minimum total water pressure load.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
