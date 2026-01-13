## Title
Construction Bricks

## Slug
construction-bricks

## Difficulty
Medium

## Description
A builder arranges bricks into pallets.

The builder has prepared $n$ bricks arranged in a sequence. The $i$-th brick has a value of $a_i$.

These bricks need to be grouped into pallets. Every pallet must hold the exact same number of bricks, denoted by $k$. The grouping happens sequentially:
- The first $k$ bricks go into the first pallet.
- The second $k$ bricks go into the second pallet.
- ...
- The last $k$ bricks go into the $(n/k)$-th pallet.

Since every pallet must have exactly $k$ bricks, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The builder wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the pallets is maximized. If there is only one pallet (i.e., $k=n$), the difference is 0.

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
- $k=1$: pallet 1 has sum 1, pallet 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one pallet with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All bricks are equal. Regardless of $k$, all pallets will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of bricks.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the bricks.

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


