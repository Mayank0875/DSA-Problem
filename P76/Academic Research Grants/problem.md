## Title
Academic Research Grants

## Slug
academic-research-grants

## Difficulty
Hard

## Description
A university has `n` research proposals. The budget is split into `k` grant buckets. Proposals are reviewed in order. The 'audit complexity' of a bucket is the square of the total funding amount in that bucket.

You must partition the sequence of proposals into exactly `k` non-empty contiguous buckets.
Each bucket corresponds to a bucket.
The "audit complexity" for a bucket is calculated as the **square of the sum** of the funding amounts of the proposals in that bucket.

Your goal is to minimize the total audit complexity (the sum of the audit complexity values of all `k` buckets).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the proposals into 3 buckets: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total audit complexity is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 bucket is allowed, containing all proposals. Sum = 15. audit complexity = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of proposals and the required number of buckets.
- The second line contains `n` integers representing the funding amounts of each proposal.

## Output Format
- Return one integer: the minimum total audit complexity.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
