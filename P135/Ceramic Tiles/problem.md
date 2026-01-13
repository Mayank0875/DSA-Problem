## Title
Ceramic Tiles

## Slug
ceramic-tiles

## Difficulty
Medium

## Description
A packer boxes tiles for shipment.

The packer has prepared $n$ tiles arranged in a sequence. The $i$-th tile has a value of $a_i$.

These tiles need to be grouped into boxes. Every box must hold the exact same number of tiles, denoted by $k$. The grouping happens sequentially:
- The first $k$ tiles go into the first box.
- The second $k$ tiles go into the second box.
- ...
- The last $k$ tiles go into the $(n/k)$-th box.

Since every box must have exactly $k$ tiles, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The packer wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the boxes is maximized. If there is only one box (i.e., $k=n$), the difference is 0.

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
- $k=1$: box 1 has sum 1, box 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one box with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All tiles are equal. Regardless of $k$, all boxes will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of tiles.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the tiles.

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


