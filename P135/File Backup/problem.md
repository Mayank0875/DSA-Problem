## Title
File Backup

## Slug
file-backup

## Difficulty
Medium

## Description
A system administrator backs up files onto disks.

The admin has prepared $n$ files arranged in a sequence. The $i$-th file has a value of $a_i$.

These files need to be grouped into disks. Every disk must hold the exact same number of files, denoted by $k$. The grouping happens sequentially:
- The first $k$ files go into the first disk.
- The second $k$ files go into the second disk.
- ...
- The last $k$ files go into the $(n/k)$-th disk.

Since every disk must have exactly $k$ files, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The admin wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the disks is maximized. If there is only one disk (i.e., $k=n$), the difference is 0.

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
- $k=1$: disk 1 has sum 1, disk 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one disk with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All files are equal. Regardless of $k$, all disks will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of files.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the files.

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


