## Title
Wine Bottling

## Slug
wine-bottling

## Difficulty
Medium

## Description
A vintner cases bottles of wine.

The vintner has prepared $n$ bottles arranged in a sequence. The $i$-th bottle has a value of $a_i$.

These bottles need to be grouped into cases. Every case must hold the exact same number of bottles, denoted by $k$. The grouping happens sequentially:
- The first $k$ bottles go into the first case.
- The second $k$ bottles go into the second case.
- ...
- The last $k$ bottles go into the $(n/k)$-th case.

Since every case must have exactly $k$ bottles, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The vintner wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the cases is maximized. If there is only one case (i.e., $k=n$), the difference is 0.

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
- $k=1$: case 1 has sum 1, case 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one case with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All bottles are equal. Regardless of $k$, all cases will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of bottles.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the bottles.

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


