## Title
Music Playlist

## Slug
music-playlist

## Difficulty
Medium

## Description
A DJ creates a setlist. Each song track has a duration in seconds.

The DJ has a sequence of tracks lined up in a row. The $i$-th track corresponds to `nums[i]` seconds.

The DJ wants to ensure if the collection contains a valid "**Perfect Loop**." A Perfect Loop is defined as a continuous sub-segment of tracks that meets two conditions:
1. The sequence must contain **at least two** tracks.
2. The total sum of the seconds in the sequence must be perfectly divisible by $k$ (the loop cycle).

Recall that 0 is always a multiple of $k$.

Your task is to determine if such a sequence exists. Return `true` if a Perfect Loop is found, and `false` otherwise.

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
- The first line contains two integers $n$ and $k$ — the number of tracks and the divisor.
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

