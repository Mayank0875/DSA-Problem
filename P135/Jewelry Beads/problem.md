## Title
Jewelry Beads

## Slug
jewelry-beads

## Difficulty
Medium

## Description
An artisan strings beads into necklaces.

The artisan has prepared $n$ beads arranged in a sequence. The $i$-th bead has a value of $a_i$.

These beads need to be grouped into necklaces. Every necklace must hold the exact same number of beads, denoted by $k$. The grouping happens sequentially:
- The first $k$ beads go into the first necklace.
- The second $k$ beads go into the second necklace.
- ...
- The last $k$ beads go into the $(n/k)$-th necklace.

Since every necklace must have exactly $k$ beads, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The artisan wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the necklaces is maximized. If there is only one necklace (i.e., $k=n$), the difference is 0.

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
- $k=1$: necklace 1 has sum 1, necklace 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one necklace with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All beads are equal. Regardless of $k$, all necklaces will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of beads.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the beads.

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


