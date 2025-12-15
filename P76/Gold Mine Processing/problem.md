## Title
Gold Mine Processing

## Slug
gold-mine-processing

## Difficulty
Hard

## Description
Miners extract `n` loads of ore with varying gold purity. They process these in `k` batches. The 'chemical waste' produced by a batch process is proportional to the square of the total purity value of that batch.

You must partition the sequence of ore loads into exactly `k` non-empty contiguous batches.
Each batch corresponds to a processing batch.
The "chemical waste" for a processing batch is calculated as the **square of the sum** of the purity values of the ore loads in that batch.

Your goal is to minimize the total chemical waste (the sum of the chemical waste values of all `k` batches).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the ore loads into 3 batches: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total chemical waste is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 batch is allowed, containing all ore loads. Sum = 15. chemical waste = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of ore loads and the required number of batches.
- The second line contains `n` integers representing the purity values of each load.

## Output Format
- Return one integer: the minimum total chemical waste.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
