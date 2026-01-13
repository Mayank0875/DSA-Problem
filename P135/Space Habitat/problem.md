## Title
Space Habitat

## Slug
space-habitat

## Difficulty
Medium

## Description
A commander assigns colonists to living modules.

The commander has prepared $n$ colonists arranged in a sequence. The $i$-th colonist has a value of $a_i$.

These colonists need to be grouped into modules. Every module must hold the exact same number of colonists, denoted by $k$. The grouping happens sequentially:
- The first $k$ colonists go into the first module.
- The second $k$ colonists go into the second module.
- ...
- The last $k$ colonists go into the $(n/k)$-th module.

Since every module must have exactly $k$ colonists, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The commander wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the modules is maximized. If there is only one module (i.e., $k=n$), the difference is 0.

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
- $k=1$: module 1 has sum 1, module 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one module with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All colonists are equal. Regardless of $k$, all modules will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of colonists.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the colonists.

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


