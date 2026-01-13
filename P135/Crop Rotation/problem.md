## Title
Crop Rotation

## Slug
crop-rotation

## Difficulty
Medium

## Description
A farmer divides a field into equal plots.

The farmer has prepared $n$ acres arranged in a sequence. The $i$-th acre has a value of $a_i$.

These acres need to be grouped into plots. Every plot must hold the exact same number of acres, denoted by $k$. The grouping happens sequentially:
- The first $k$ acres go into the first plot.
- The second $k$ acres go into the second plot.
- ...
- The last $k$ acres go into the $(n/k)$-th plot.

Since every plot must have exactly $k$ acres, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The farmer wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the plots is maximized. If there is only one plot (i.e., $k=n$), the difference is 0.

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
- $k=1$: plot 1 has sum 1, plot 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one plot with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All acres are equal. Regardless of $k$, all plots will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of acres.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the acres.

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


