## Title
Fireworks Display

## Slug
fireworks-display

## Difficulty
Medium

## Description
A pyrotechnician wires shells into firing cues.

The technician has prepared $n$ shells arranged in a sequence. The $i$-th shell has a value of $a_i$.

These shells need to be grouped into cues. Every cue must hold the exact same number of shells, denoted by $k$. The grouping happens sequentially:
- The first $k$ shells go into the first cue.
- The second $k$ shells go into the second cue.
- ...
- The last $k$ shells go into the $(n/k)$-th cue.

Since every cue must have exactly $k$ shells, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The technician wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the cues is maximized. If there is only one cue (i.e., $k=n$), the difference is 0.

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
- $k=1$: cue 1 has sum 1, cue 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one cue with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All shells are equal. Regardless of $k$, all cues will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of shells.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the shells.

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


