## Title
Lumber Yard

## Slug
lumber-yard

## Difficulty
Medium

## Description
A logger bundles logs for transport.

The logger has prepared $n$ logs arranged in a sequence. The $i$-th log has a value of $a_i$.

These logs need to be grouped into bundles. Every bundle must hold the exact same number of logs, denoted by $k$. The grouping happens sequentially:
- The first $k$ logs go into the first bundle.
- The second $k$ logs go into the second bundle.
- ...
- The last $k$ logs go into the $(n/k)$-th bundle.

Since every bundle must have exactly $k$ logs, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The logger wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the bundles is maximized. If there is only one bundle (i.e., $k=n$), the difference is 0.

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
All logs are equal. Regardless of $k$, all bundles will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of logs.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the logs.

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


