## Title
Donation Sorting

## Slug
donation-sorting

## Difficulty
Medium

## Description
A volunteer packs donated items into care packages.

The volunteer has prepared $n$ items arranged in a sequence. The $i$-th item has a value of $a_i$.

These items need to be grouped into packages. Every package must hold the exact same number of items, denoted by $k$. The grouping happens sequentially:
- The first $k$ items go into the first package.
- The second $k$ items go into the second package.
- ...
- The last $k$ items go into the $(n/k)$-th package.

Since every package must have exactly $k$ items, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The volunteer wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the packages is maximized. If there is only one package (i.e., $k=n$), the difference is 0.

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
- $k=1$: package 1 has sum 1, package 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one package with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All items are equal. Regardless of $k$, all packages will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of items.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the items.

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


