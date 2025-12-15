## Title
Grain Silo storage

## Slug
grain-silo-storage

## Difficulty
Hard

## Description
A farmer fills `k` silos with `n` harvests of varying tonnage. Harvests are loaded sequentially. The 'compaction force' at the bottom of a silo is the square of the total weight stored in it.

You must partition the sequence of harvests into exactly `k` non-empty contiguous loads.
Each load corresponds to a silo.
The "compaction force" for a silo is calculated as the **square of the sum** of the weights of the harvests in that load.

Your goal is to minimize the total compaction force (the sum of the compaction force values of all `k` loads).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the harvests into 3 loads: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total compaction force is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 load is allowed, containing all harvests. Sum = 15. compaction force = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of harvests and the required number of loads.
- The second line contains `n` integers representing the weights of each harvest.

## Output Format
- Return one integer: the minimum total compaction force.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
