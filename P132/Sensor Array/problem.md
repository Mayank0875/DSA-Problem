## Title
Sensor Array

## Slug
sensor-array

## Difficulty
Medium

## Description
Seismic sensors transmit warnings. Signals must propagate to the Alert Center.

There are $n$ sensors numbered from $1$ to $n$, connected by $n-1$ wires. The network forms a tree structure (there is exactly one path between any two sensors). Currently, all wires are one-way.

Safety protocols require data routing to the **Alert Center (Node 1)**. To ensure success, every other sensor must be able to reach Alert Center by traveling along the wires in the correct direction.

You are given the current orientation of the wires. Your task is to determine the **minimum** number of wires that need to be soldered differently so that every sensor can reach Alert Center.

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
The destination is Alert Center (1).
- Wire 1->2 points away from 1. Needs change.
- Wire 2->4 points away from 1. Needs change.
- Wire 3->2 points towards 2 (and effectively towards 1). OK.
- Wire 5->1 points towards 1. OK.
- Wire 5->6 points away from 1 (via 5). Needs change.
Total changes: 3.

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
Wires 2->3 and 4->5 need to be changed.

## Input Format
- The first line contains an integer $n$ — the number of sensors.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way wire from sensor $u$ to sensor $v$.

## Output Format
- Return a single integer representing the minimum number of wires that need to be changed.

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
