## Title
Electricity Usage

## Slug
electricity-usage

## Difficulty
Medium

## Description
A smart meter records hourly energy consumption.

The auditor has a sequence of hours lined up in a row. The $i$-th hour corresponds to `nums[i]` kilowatts.

The auditor wants to calculate if the collection contains a valid "**Billable Block**." A Billable Block is defined as a continuous sub-segment of hours that meets two conditions:
1. The sequence must contain **at least two** hours.
2. The total sum of the kilowatts in the sequence must be perfectly divisible by $k$ (the billing threshold).

Recall that 0 is always a multiple of $k$.

Your task is to determine if such a sequence exists. Return `true` if a Billable Block is found, and `false` otherwise.

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
- The first line contains two integers $n$ and $k$ — the number of hours and the divisor.
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

