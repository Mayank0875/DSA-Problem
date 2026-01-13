## Title
Memory Allocation

## Slug
memory-allocation

## Difficulty
Medium

## Description
An OS kernel divides memory bytes into pages.

The kernel has prepared $n$ bytes arranged in a sequence. The $i$-th byte has a value of $a_i$.

These bytes need to be grouped into pages. Every page must hold the exact same number of bytes, denoted by $k$. The grouping happens sequentially:
- The first $k$ bytes go into the first page.
- The second $k$ bytes go into the second page.
- ...
- The last $k$ bytes go into the $(n/k)$-th page.

Since every page must have exactly $k$ bytes, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The kernel wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the pages is maximized. If there is only one page (i.e., $k=n$), the difference is 0.

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
- $k=1$: page 1 has sum 1, page 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one page with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All bytes are equal. Regardless of $k$, all pages will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of bytes.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the bytes.

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


