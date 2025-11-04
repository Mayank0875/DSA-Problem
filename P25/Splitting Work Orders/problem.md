## Title

Splitting Work Orders

## Slug

splitting-work-orders

## Difficulty

Medium

## Description

A manager has `n` work orders that must be processed sequentially. Order `i` has a complexity of `x[i]`. These orders must be distributed among `k` available teams. Each team must handle a contiguous block of orders. To keep the workflow smooth, the manager wants to minimize the maximum total complexity handled by any single team. Find this minimum-maximum value.

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

- The first line contains two integers `n` and `k`: the number of work orders and the number of teams.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the complexity of the i-th order.

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