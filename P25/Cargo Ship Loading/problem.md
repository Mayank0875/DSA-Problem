## Title

Cargo Ship Loading

## Slug

cargo-ship-loading

## Difficulty

Medium

## Description

You need to load `n` containers, lined up on a dock, onto `k` cargo ships. Each container `i` has a weight of `x[i]`. Each ship must take a contiguous block of containers (e.g., ship 1 takes containers 1 to `j`, ship 2 takes `j+1` to `m`, etc.). To keep the ships balanced, you must find a way to distribute the containers that minimizes the maximum weight any single ship has to carry. Find this minimum-maximum weight.

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

- The first line contains two integers `n` and `k`: the number of containers and the number of ships.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the weight of the i-th container.

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