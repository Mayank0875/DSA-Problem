## Title
Fishing Net

## Slug
fishing-net

## Difficulty
Medium

## Description
A fisherman sorts fish into buckets.

The fisherman has prepared $n$ fish arranged in a sequence. The $i$-th fish has a value of $a_i$.

These fish need to be grouped into buckets. Every bucket must hold the exact same number of fish, denoted by $k$. The grouping happens sequentially:
- The first $k$ fish go into the first bucket.
- The second $k$ fish go into the second bucket.
- ...
- The last $k$ fish go into the $(n/k)$-th bucket.

Since every bucket must have exactly $k$ fish, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The fisherman wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the buckets is maximized. If there is only one bucket (i.e., $k=n$), the difference is 0.

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
- $k=1$: bucket 1 has sum 1, bucket 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one bucket with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All fish are equal. Regardless of $k$, all buckets will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of fish.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the fish.

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


