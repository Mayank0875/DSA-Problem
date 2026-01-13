## Title
Music Playlist

## Slug
music-playlist

## Difficulty
Medium

## Description
A DJ groups songs into sets for a show.

The DJ has prepared $n$ songs arranged in a sequence. The $i$-th song has a value of $a_i$.

These songs need to be grouped into sets. Every set must hold the exact same number of songs, denoted by $k$. The grouping happens sequentially:
- The first $k$ songs go into the first set.
- The second $k$ songs go into the second set.
- ...
- The last $k$ songs go into the $(n/k)$-th set.

Since every set must have exactly $k$ songs, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The DJ wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the sets is maximized. If there is only one set (i.e., $k=n$), the difference is 0.

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
- $k=1$: set 1 has sum 1, set 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one set with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All songs are equal. Regardless of $k$, all sets will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of songs.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the songs.

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


