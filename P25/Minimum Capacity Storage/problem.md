## Title

Minimum Capacity Storage

## Slug

minimum-capacity-storage

## Difficulty

Medium

## Description

You have `n` data files, ordered by time, with sizes `x[i]`. You need to archive these files onto `k` identical storage disks. Each disk must store a contiguous block of files (e.g., disk 1 stores files 1-3, disk 2 stores 4-7, etc.). To save money, you want to buy `k` disks of the smallest possible, identical capacity. What is the minimum capacity `C` such that you can store all files, where `C` is the maximum total size on any single disk?

## Examples

### 1

#### Input

5 3 
2 4 7 3 5


#### Output

8

#### Explanation

An optimal distribution assigns scrolls [2, 4] to the first scribe (sum 6 pages), scroll [7] to the second scribe (sum 7 pages), and scrolls [3, 5] to the third scribe (sum 8 pages). The maximum number of pages assigned to any scribe is 8. No other distribution into 3 contiguous blocks can achieve a maximum load less than 8.

### 2

#### Input

1 1
34

#### Output

34


#### Explanation

No other distribution into 1 contiguous blocks can achieve a maximum load less than 34.

## Input Format

- The first line contains two integers `n` and `k`: the number of files and the number of disks.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the size of the i-th file.

## Output Format

- Return one integer: the minimum possible value for the maximum number of pages assigned to any scribe.

## Constraints

- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ x[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, greedy