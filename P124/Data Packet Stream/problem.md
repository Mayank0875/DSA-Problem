## Title
Data Packet Stream

## Slug
data-packet-stream

## Difficulty
Medium

## Description
A network analyzer monitors a stream of data packets. Each packet has a specific byte size.

The admin has a sequence of packets lined up in a row. The $i$-th packet corresponds to `nums[i]` bytes.

The admin wants to detect if the collection contains a valid "**Clean Frame**." A Clean Frame is defined as a continuous sub-segment of packets that meets two conditions:
1. The sequence must contain **at least two** packets.
2. The total sum of the bytes in the sequence must be perfectly divisible by $k$ (the buffer limit).

Recall that 0 is always a multiple of $k$.

Your task is to determine if such a sequence exists. Return `true` if a Clean Frame is found, and `false` otherwise.

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
- The first line contains two integers $n$ and $k$ — the number of packets and the divisor.
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

