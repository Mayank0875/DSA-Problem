## Title

Factory Production Quotas

## Slug

factory-production-quotas

## Difficulty

Medium

## Description

A factory has `n` assembly jobs lined up for the day, in a fixed order. Job `i` requires `x[i]` minutes to complete. The factory manager needs to assign these jobs to `k` available production lines. Each line must handle a contiguous block of jobs. The manager wants to minimize the completion time of the entire batch, which is determined by the production line with the largest total workload. Find the minimum possible time for the busiest production line.

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

- The first line contains two integers `n` and `k`: the number of jobs and the number of production lines.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the time in minutes for the i-th job.

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