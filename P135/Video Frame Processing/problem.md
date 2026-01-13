## Title
Video Frame Processing

## Slug
video-frame-processing

## Difficulty
Medium

## Description
A video editor processes frames in chunks.

The editor has prepared $n$ frames arranged in a sequence. The $i$-th frame has a value of $a_i$.

These frames need to be grouped into chunks. Every chunk must hold the exact same number of frames, denoted by $k$. The grouping happens sequentially:
- The first $k$ frames go into the first chunk.
- The second $k$ frames go into the second chunk.
- ...
- The last $k$ frames go into the $(n/k)$-th chunk.

Since every chunk must have exactly $k$ frames, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The editor wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the chunks is maximized. If there is only one chunk (i.e., $k=n$), the difference is 0.

Your task is to calculate this maximum possible difference over all valid choices of $k$.

## Examples

### 1

#### Input
2
1 2

#### Output
1

#### Explanation
Possible values for $k$ are divisors of 2: 1, 2.
- $k=1$: chunk 1 has sum 1, chunk 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one chunk with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All frames are equal. Regardless of $k$, all chunks will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of frames.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the frames.

## Output Format
- Return a single integer — the maximum absolute difference.

## Constraints
- 1 ≤ n ≤ 1.5 * 10^5
- 1 ≤ a[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, math, number-theory


