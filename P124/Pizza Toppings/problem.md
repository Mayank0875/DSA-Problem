## Title
Pizza Toppings

## Slug
pizza-toppings

## Difficulty
Medium

## Description
A chef counts pepperoni slices on different pizza slices.

The chef has a sequence of slices lined up in a row. The $i$-th slice corresponds to `nums[i]` pepperonis.

The chef wants to verify if the collection contains a valid "**Fair Portion**." A Fair Portion is defined as a continuous sub-segment of slices that meets two conditions:
1. The sequence must contain **at least two** slices.
2. The total sum of the pepperonis in the sequence must be perfectly divisible by $k$ (the serving portion).

Recall that 0 is always a multiple of $k$.

Your task is to determine if such a sequence exists. Return `true` if a Fair Portion is found, and `false` otherwise.

## Examples

### 1

#### Input
5 6
23 2 4 6 7

#### Output
true

#### Explanation
The subsequence `[2, 4]` sums to 6.
6 is a multiple of 6.
The length is 2, which satisfies the condition.

### 2

#### Input
5 13
23 2 6 4 7

#### Output
false

#### Explanation
No continuous subarray of length at least 2 has a sum divisible by 13.

## Input Format
- The first line contains two integers $n$ and $k$ — the number of slices and the divisor.
- The second line contains $n$ space-separated integers, representing the values.

## Output Format
- Return `true` if a valid subarray exists, otherwise return `false`.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ k ≤ 10^9
- 0 ≤ nums[i] ≤ 10^9
- The sum of elements will fit within a 64-bit integer.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
hash-table, prefix-sum, math, array

