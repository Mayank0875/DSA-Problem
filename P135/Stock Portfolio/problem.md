## Title
Stock Portfolio

## Slug
stock-portfolio

## Difficulty
Medium

## Description
An investor groups stocks into diverse funds.

The investor has prepared $n$ stocks arranged in a sequence. The $i$-th stock has a value of $a_i$.

These stocks need to be grouped into funds. Every fund must hold the exact same number of stocks, denoted by $k$. The grouping happens sequentially:
- The first $k$ stocks go into the first fund.
- The second $k$ stocks go into the second fund.
- ...
- The last $k$ stocks go into the $(n/k)$-th fund.

Since every fund must have exactly $k$ stocks, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The investor wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the funds is maximized. If there is only one fund (i.e., $k=n$), the difference is 0.

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
- $k=1$: fund 1 has sum 1, fund 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one fund with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All stocks are equal. Regardless of $k$, all funds will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of stocks.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the stocks.

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


