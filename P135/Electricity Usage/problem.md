## Title
Electricity Usage

## Slug
electricity-usage

## Difficulty
Medium

## Description
An analyst groups hourly energy readings into time blocks.

The analyst has prepared $n$ readings arranged in a sequence. The $i$-th reading has a value of $a_i$.

These readings need to be grouped into blocks. Every block must hold the exact same number of readings, denoted by $k$. The grouping happens sequentially:
- The first $k$ readings go into the first block.
- The second $k$ readings go into the second block.
- ...
- The last $k$ readings go into the $(n/k)$-th block.

Since every block must have exactly $k$ readings, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The analyst wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the blocks is maximized. If there is only one block (i.e., $k=n$), the difference is 0.

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
- $k=1$: block 1 has sum 1, block 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one block with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All readings are equal. Regardless of $k$, all blocks will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of readings.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the readings.

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


