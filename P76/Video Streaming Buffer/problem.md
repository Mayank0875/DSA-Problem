## Title
Video Streaming Buffer

## Slug
video-streaming-buffer

## Difficulty
Hard

## Description
A video player downloads `n` frame chunks to play over `k` buffering intervals. Each chunk has a data size. Chunks are grouped contiguously. The 'lag potential' for an interval is the square of the total data size buffered.

You must partition the sequence of frame chunks into exactly `k` non-empty contiguous intervals.
Each interval corresponds to a buffer interval.
The "lag potential" for a buffer interval is calculated as the **square of the sum** of the data sizes of the frame chunks in that interval.

Your goal is to minimize the total lag potential (the sum of the lag potential values of all `k` intervals).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the frame chunks into 3 intervals: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total lag potential is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 interval is allowed, containing all frame chunks. Sum = 15. lag potential = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of frame chunks and the required number of intervals.
- The second line contains `n` integers representing the data sizes of each chunk.

## Output Format
- Return one integer: the minimum total lag potential.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
