## Title

Fair Task Delegation

## Slug

fair-task-delegation

## Difficulty

Medium

## Description

You have `n` tasks in a queue, where task `i` has a difficulty `x[i]`. You need to assign these tasks to `k` employees. Each employee must take a contiguous set of tasks from the queue (e.g., employee 1 takes tasks 1-`j`, employee 2 takes `j+1`-`m`). You want to be a fair boss, so you must minimize the maximum total difficulty assigned to any single employee. Find this minimum-maximum difficulty.

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

- The first line contains two integers `n` and `k`: the number of tasks and the number of employees.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the difficulty of the i-th task.

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