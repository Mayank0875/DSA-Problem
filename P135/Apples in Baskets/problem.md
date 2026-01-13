## Title
Apples in Baskets

## Slug
apples-in-baskets

## Difficulty
Medium

## Description
A picker puts apples into baskets.

The picker has prepared $n$ apples arranged in a sequence. The $i$-th apple has a value of $a_i$.

These apples need to be grouped into baskets. Every basket must hold the exact same number of apples, denoted by $k$. The grouping happens sequentially:
- The first $k$ apples go into the first basket.
- The second $k$ apples go into the second basket.
- ...
- The last $k$ apples go into the $(n/k)$-th basket.

Since every basket must have exactly $k$ apples, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The picker wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the baskets is maximized. If there is only one basket (i.e., $k=n$), the difference is 0.

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
- $k=1$: basket 1 has sum 1, basket 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one basket with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All apples are equal. Regardless of $k$, all baskets will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of apples.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the apples.

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


