## Title

Splitting the Log File

## Slug

splitting-the-log-file

## Difficulty

Medium

## Description

A server has generated a large log file, which can be seen as `n` sequential blocks. Block `i` has size `x[i]`. You need to split this log file into `k` smaller, contiguous parts to be analyzed by `k` different processes. To balance the work, you must minimize the maximum size of any part. Find the minimum possible value for the largest part.

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

- The first line contains two integers `n` and `k`: the number of blocks and the number of parts.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the size of the i-th block.

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