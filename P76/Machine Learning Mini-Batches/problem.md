## Title
Machine Learning Mini-Batches

## Slug
machine-learning-mini-batches

## Difficulty
Hard

## Description
A training dataset has `n` samples. The model processes them in `k` mini-batches. Samples have different vector lengths. The 'computation spike' for a batch is the square of the sum of vector lengths in that batch.

You must partition the sequence of samples into exactly `k` non-empty contiguous batches.
Each batch corresponds to a mini-batch.
The "computation spike" for a mini-batch is calculated as the **square of the sum** of the vector lengths of the samples in that batch.

Your goal is to minimize the total computation spike (the sum of the computation spike values of all `k` batches).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the samples into 3 batches: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total computation spike is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 batch is allowed, containing all samples. Sum = 15. computation spike = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of samples and the required number of batches.
- The second line contains `n` integers representing the vector lengths of each sample.

## Output Format
- Return one integer: the minimum total computation spike.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
