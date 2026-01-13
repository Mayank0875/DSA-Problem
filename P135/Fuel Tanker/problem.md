## Title
Fuel Tanker

## Slug
fuel-tanker

## Difficulty
Medium

## Description
A refinery fills tanker trucks with oil barrels.

The manager has prepared $n$ barrels arranged in a sequence. The $i$-th barrel has a value of $a_i$.

These barrels need to be grouped into trucks. Every truck must hold the exact same number of barrels, denoted by $k$. The grouping happens sequentially:
- The first $k$ barrels go into the first truck.
- The second $k$ barrels go into the second truck.
- ...
- The last $k$ barrels go into the $(n/k)$-th truck.

Since every truck must have exactly $k$ barrels, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The manager wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the trucks is maximized. If there is only one truck (i.e., $k=n$), the difference is 0.

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
- $k=1$: truck 1 has sum 1, truck 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one truck with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All barrels are equal. Regardless of $k$, all trucks will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of barrels.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the barrels.

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


