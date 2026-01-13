## Title
Gold Bar Stacking

## Slug
gold-bar-stacking

## Difficulty
Medium

## Description
A banker organizes gold bars into secure vaults.

The banker has prepared $n$ gold bars arranged in a sequence. The $i$-th bar has a value of $a_i$.

These gold bars need to be grouped into vaults. Every vault must hold the exact same number of gold bars, denoted by $k$. The grouping happens sequentially:
- The first $k$ gold bars go into the first vault.
- The second $k$ gold bars go into the second vault.
- ...
- The last $k$ gold bars go into the $(n/k)$-th vault.

Since every vault must have exactly $k$ gold bars, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The banker wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the vaults is maximized. If there is only one vault (i.e., $k=n$), the difference is 0.

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
- $k=1$: vault 1 has sum 1, vault 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one vault with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All gold bars are equal. Regardless of $k$, all vaults will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of gold bars.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the gold bars.

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


