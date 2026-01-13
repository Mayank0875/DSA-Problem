## Title
Signal Processing

## Slug
signal-processing

## Difficulty
Medium

## Description
A DSP chip processes samples in windows.

The chip has prepared $n$ samples arranged in a sequence. The $i$-th sample has a value of $a_i$.

These samples need to be grouped into windows. Every window must hold the exact same number of samples, denoted by $k$. The grouping happens sequentially:
- The first $k$ samples go into the first window.
- The second $k$ samples go into the second window.
- ...
- The last $k$ samples go into the $(n/k)$-th window.

Since every window must have exactly $k$ samples, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The chip wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the windows is maximized. If there is only one window (i.e., $k=n$), the difference is 0.

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
- $k=1$: window 1 has sum 1, window 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one window with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All samples are equal. Regardless of $k$, all windows will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of samples.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the samples.

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


