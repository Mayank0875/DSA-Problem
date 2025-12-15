## Title
Restaurant Table Seating

## Slug
restaurant-table-seating

## Difficulty
Hard

## Description
A party of `n` sub-groups arrives. They are seated at `k` large tables. Sub-groups stay together in arrival order. The 'noise generation' of a table is the square of the total number of people seated there.

You must partition the sequence of sub-groups into exactly `k` non-empty contiguous tables.
Each table corresponds to a table.
The "noise generation" for a table is calculated as the **square of the sum** of the counts of the sub-groups in that table.

Your goal is to minimize the total noise generation (the sum of the noise generation values of all `k` tables).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the sub-groups into 3 tables: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total noise generation is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 table is allowed, containing all sub-groups. Sum = 15. noise generation = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of sub-groups and the required number of tables.
- The second line contains `n` integers representing the counts of each sub-group.

## Output Format
- Return one integer: the minimum total noise generation.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
