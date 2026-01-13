## Title
Election Ballots

## Slug
election-ballots

## Difficulty
Medium

## Description
An official bundles ballots for counting.

The official has prepared $n$ ballots arranged in a sequence. The $i$-th ballot has a value of $a_i$.

These ballots need to be grouped into bundles. Every bundle must hold the exact same number of ballots, denoted by $k$. The grouping happens sequentially:
- The first $k$ ballots go into the first bundle.
- The second $k$ ballots go into the second bundle.
- ...
- The last $k$ ballots go into the $(n/k)$-th bundle.

Since every bundle must have exactly $k$ ballots, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The official wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the bundles is maximized. If there is only one bundle (i.e., $k=n$), the difference is 0.

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
- $k=1$: bundle 1 has sum 1, bundle 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one bundle with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All ballots are equal. Regardless of $k$, all bundles will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of ballots.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the ballots.

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


