## Title
Charity Runs

## Slug
charity-runs

## Difficulty
Medium

## Description
An organizer groups runners into heats.

The organizer has prepared $n$ runners arranged in a sequence. The $i$-th runner has a value of $a_i$.

These runners need to be grouped into heats. Every heat must hold the exact same number of runners, denoted by $k$. The grouping happens sequentially:
- The first $k$ runners go into the first heat.
- The second $k$ runners go into the second heat.
- ...
- The last $k$ runners go into the $(n/k)$-th heat.

Since every heat must have exactly $k$ runners, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The organizer wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the heats is maximized. If there is only one heat (i.e., $k=n$), the difference is 0.

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
- $k=1$: heat 1 has sum 1, heat 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one heat with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All runners are equal. Regardless of $k$, all heats will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of runners.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the runners.

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


