## Title

Server Load Balancing

## Slug

server-load-balancing

## Difficulty

Medium

## Description

You have `n` data packets that must be processed in order. Packet `i` has a size of `x[i]`. You have `k` servers to process this data. You must assign a contiguous block of packets to each server (e.g., server 1 gets packets 1-`j`, server 2 gets `j+1` to `m`, etc.). Your goal is to minimize the maximum load (total data size) on any single server. Find the minimum possible value for this maximum load.

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

- The first line contains two integers `n` and `k`: the number of packets and the number of servers.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the size of the i-th packet.

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