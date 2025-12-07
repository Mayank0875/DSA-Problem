## Title
Airline Route Hubs

## Slug
airline-route-hubs

## Difficulty
Medium

## Description
An airline flies to n cities. Planners identify hubs connecting groups of k destinations.

The Planner defines the "Hub Centrality" of the structure rooted at a specific city `r` as follows:
Consider every possible set of `k` distinct cities from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the cities in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique cities obtained as LCAs from these sets.
3. The Hub Centrality of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Network Connectivity" is defined as the sum of the Hub Centrality values for all possible roots `r` from 1 to `n`:
Network Connectivity = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Network Connectivity of the given route map.

Notes:
1. A route map is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted route map is the deepest node that is an ancestor of all nodes in the set.

## Examples

### 1

#### Input
6 3
1 2
1 3
2 4
2 5
3 6

#### Output
17

#### Explanation
The calculated Network Connectivity is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Network Connectivity is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of cities and the size of the sets to consider.
- The following `n-1` lines describe the route map. Each line contains two integers `u` and `v`, indicating a connection between cities `u` and `v`.

## Output Format
- Return one integer: the Network Connectivity.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
