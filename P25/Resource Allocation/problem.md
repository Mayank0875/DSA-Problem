## Title

Resource Allocation

## Slug

resource-allocation

## Difficulty

Medium

## Description

You have `n` tasks in a sequence. Task `i` requires `x[i]` units of a resource. You need to allocate these tasks to `k` workers. Each worker must handle a contiguous block of tasks. Your goal is to minimize the resource consumption of the most heavily-loaded worker. Find the minimum possible value for the maximum resource units assigned to any single worker.

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

- The first line contains two integers `n` and `k`: the number of tasks and the number of workers.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the resource cost of the i-th task.

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