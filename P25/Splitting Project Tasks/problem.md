## Title

Splitting Project Tasks

## Slug

splitting-project-tasks

## Difficulty

Medium

## Description

A project manager has `n` sequential tasks that must be completed. Each task `i` has an estimated workload of `x[i]` hours. These tasks must be divided among `k` available programmers. Each programmer must be assigned a contiguous block of tasks (e.g., programmer 1 takes tasks 1-3, programmer 2 takes 4-5, etc.). To ensure fairness and avoid burnout, the manager wants to minimize the maximum total hours assigned to any single programmer. Find this minimum-maximum workload.

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

- The first line contains two integers `n` and `k`: the number of tasks and the number of programmers.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the hour-workload of the i-th task.

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