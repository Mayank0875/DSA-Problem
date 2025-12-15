## Title
Cave Spelunking

## Slug
cave-spelunking

## Difficulty
Medium

## Description
An explorer crawls from Entrance 1 to Exit n.

The cave system has `n` caverns and `m` directed tunnels. Tunnels may repeat between the same pair of caverns and self-loops are allowed. A exploration of length `k` is a sequence of exactly `k` directed tunnels; caverns and tunnels may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed tunnels (each tunnel given as two integers `u` `v` meaning a directed tunnel from `u` to `v`), compute the number of distinct explorations that start at cavern 1 and end at cavern `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 caverns. We want the number of directed explorations of length 8 from cavern 1 to cavern 3.
Valid length-8 explorations:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such explorations.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has tunnels 1->2 and 2->3, the only exploration of length 2 from cavern 1 to cavern 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of caverns, tunnels, and the required exploration length.
- The next m lines describe the tunnels. Each line contains two integers u and v, indicating a directed tunnel from cavern u to cavern v.

## Output Format
- Return single integer: the number of explorations modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
