## Title

Relay Race Team

## Slug

relay-race-team

## Difficulty

Medium

## Description

You are organizing a `k`-person relay race. The race course consists of `n` sequential segments, with segment `i` having a difficulty of `x[i]`. Each of the `k` runners must run a contiguous block of one or more segments (e.g., runner 1 does 1-2, runner 2 does 3, runner 3 does 4-5, etc.). To make the race fair, you want to minimize the maximum total difficulty assigned to any single runner. Find this minimum-maximum difficulty.

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

- The first line contains two integers `n` and `k`: the number of segments and the number of runners.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the difficulty of the i-th segment.

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