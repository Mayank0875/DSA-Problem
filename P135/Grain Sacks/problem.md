## Title
Grain Sacks

## Slug
grain-sacks

## Difficulty
Medium

## Description
A miller loads sacks of grain into wagons.

The miller has prepared $n$ sacks arranged in a sequence. The $i$-th sack has a value of $a_i$.

These sacks need to be grouped into wagons. Every wagon must hold the exact same number of sacks, denoted by $k$. The grouping happens sequentially:
- The first $k$ sacks go into the first wagon.
- The second $k$ sacks go into the second wagon.
- ...
- The last $k$ sacks go into the $(n/k)$-th wagon.

Since every wagon must have exactly $k$ sacks, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The miller wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the wagons is maximized. If there is only one wagon (i.e., $k=n$), the difference is 0.

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
- $k=1$: wagon 1 has sum 1, wagon 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one wagon with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All sacks are equal. Regardless of $k$, all wagons will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of sacks.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the sacks.

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


