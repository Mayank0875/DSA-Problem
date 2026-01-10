## Title
Emergency Calls

## Slug
emergency-calls

## Difficulty
Medium

## Description
Call towers relay signals. All 911 calls must route to the Dispatch Center.

There are $n$ towers numbered from $1$ to $n$, connected by $n-1$ relays. The network forms a tree structure (there is exactly one path between any two towers). Currently, all relays are one-way.

The emergency grid directs calls to the **Dispatch Center (Node 1)**. To ensure success, every other tower must be able to reach Dispatch Center by traveling along the relays in the correct direction.

You are given the current orientation of the relays. Your task is to determine the **minimum** number of relays that need to be reprogrammed so that every tower can reach Dispatch Center.

## Examples

### 1

#### Input
6
1 2
2 4
3 2
5 1
5 6

#### Output
3

#### Explanation
The destination is Dispatch Center (1).
- Relay 1->2 points away from 1. Needs reprogramming.
- Relay 2->4 points away from 1. Needs reprogramming.
- Relay 3->2 points towards 2 (and effectively towards 1). OK.
- Relay 5->1 points towards 1. OK.
- Relay 5->6 points away from 1 (via 5). Needs reprogramming.
Total reprogrammings: 3.

### 2

#### Input
5
2 1
2 3
4 3
4 5

#### Output
2

#### Explanation
Relays 2->3 and 4->5 need to be reprogrammed.

## Input Format
- The first line contains an integer $n$ — the number of towers.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way relay from tower $u$ to tower $v$.

## Output Format
- Return a single integer representing the minimum number of relays that need to be changed.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ u, v ≤ n
- The graph is guaranteed to be a tree.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
tree, depth-first-search, breadth-first-search, graph

## Company
google, amazon
