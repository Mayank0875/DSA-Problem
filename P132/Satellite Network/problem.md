## Title
Satellite Network

## Slug
satellite-network

## Difficulty
Medium

## Description
A constellation of satellites uses laser links. All telemetry data must hop to the Ground Uplink Satellite.

There are $n$ satellites numbered from $1$ to $n$, connected by $n-1$ laser links. The network forms a tree structure (there is exactly one path between any two satellites). Currently, all laser links are one-way.

The network topology must route to the **Ground Uplink (Node 1)**. To ensure success, every other satellite must be able to reach Ground Uplink by traveling along the laser links in the correct direction.

You are given the current orientation of the laser links. Your task is to determine the **minimum** number of laser links that need to be realigned so that every satellite can reach Ground Uplink.

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
The destination is Ground Uplink (1).
- Link 1->2 points away from 1. Needs realignment.
- Link 2->4 points away from 1. Needs realignment.
- Link 3->2 points towards 2 (and effectively towards 1). OK.
- Link 5->1 points towards 1. OK.
- Link 5->6 points away from 1 (via 5). Needs realignment.
Total realignments: 3.

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
Links 2->3 and 4->5 need to be realigned.

## Input Format
- The first line contains an integer $n$ — the number of satellites.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way laser link from satellite $u$ to satellite $v$.

## Output Format
- Return a single integer representing the minimum number of laser links that need to be changed.

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
