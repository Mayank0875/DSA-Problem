## Title
Harvest Collection

## Slug
harvest-collection

## Difficulty
Medium

## Description
A farmer divides harvested pumpkins into equal crates.

The farmer has prepared $n$ pumpkins arranged in a sequence. The $i$-th pumpkin has a value of $a_i$.

These pumpkins need to be grouped into crates. Every crate must hold the exact same number of pumpkins, denoted by $k$. The grouping happens sequentially:
- The first $k$ pumpkins go into the first crate.
- The second $k$ pumpkins go into the second crate.
- ...
- The last $k$ pumpkins go into the $(n/k)$-th crate.

Since every crate must have exactly $k$ pumpkins, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The farmer wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the crates is maximized. If there is only one crate (i.e., $k=n$), the difference is 0.

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
- $k=1$: crate 1 has sum 1, crate 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one crate with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All pumpkins are equal. Regardless of $k$, all crates will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of pumpkins.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the pumpkins.

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


