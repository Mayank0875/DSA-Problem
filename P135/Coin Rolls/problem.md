## Title
Coin Rolls

## Slug
coin-rolls

## Difficulty
Medium

## Description
A cashier rolls coins into wrappers.

The cashier has prepared $n$ coins arranged in a sequence. The $i$-th coin has a value of $a_i$.

These coins need to be grouped into wrappers. Every wrapper must hold the exact same number of coins, denoted by $k$. The grouping happens sequentially:
- The first $k$ coins go into the first wrapper.
- The second $k$ coins go into the second wrapper.
- ...
- The last $k$ coins go into the $(n/k)$-th wrapper.

Since every wrapper must have exactly $k$ coins, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The cashier wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the wrappers is maximized. If there is only one wrapper (i.e., $k=n$), the difference is 0.

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
- $k=1$: wrapper 1 has sum 1, wrapper 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one wrapper with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All coins are equal. Regardless of $k$, all wrappers will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of coins.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the coins.

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


