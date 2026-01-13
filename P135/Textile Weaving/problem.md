## Title
Textile Weaving

## Slug
textile-weaving

## Difficulty
Medium

## Description
A weaver groups threads into patterns.

The weaver has prepared $n$ threads arranged in a sequence. The $i$-th thread has a value of $a_i$.

These threads need to be grouped into patterns. Every pattern must hold the exact same number of threads, denoted by $k$. The grouping happens sequentially:
- The first $k$ threads go into the first pattern.
- The second $k$ threads go into the second pattern.
- ...
- The last $k$ threads go into the $(n/k)$-th pattern.

Since every pattern must have exactly $k$ threads, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The weaver wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the patterns is maximized. If there is only one pattern (i.e., $k=n$), the difference is 0.

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
- $k=1$: pattern 1 has sum 1, pattern 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one pattern with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All threads are equal. Regardless of $k$, all patterns will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of threads.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the threads.

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


