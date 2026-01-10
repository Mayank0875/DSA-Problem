## Title
Video Streaming

## Slug
video-streaming

## Difficulty
Medium

## Description
Data buffers through nodes. All chunks must stream to the User Device.

There are $n$ cache nodes numbered from $1$ to $n$, connected by $n-1$ streams. The network forms a tree structure (there is exactly one path between any two cache nodes). Currently, all streams are one-way.

The CDN pushes data to the **User Device (Node 1)**. To ensure success, every other node must be able to reach User Device by traveling along the streams in the correct direction.

You are given the current orientation of the streams. Your task is to determine the **minimum** number of streams that need to be routed so that every node can reach User Device.

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
The destination is User Device (1).
- Stream 1->2 points away from 1. Needs routing.
- Stream 2->4 points away from 1. Needs routing.
- Stream 3->2 points towards 2 (and effectively towards 1). OK.
- Stream 5->1 points towards 1. OK.
- Stream 5->6 points away from 1 (via 5). Needs routing.
Total routings: 3.

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
Streams 2->3 and 4->5 need to be routed.

## Input Format
- The first line contains an integer $n$ — the number of cache nodes.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way stream from node $u$ to node $v$.

## Output Format
- Return a single integer representing the minimum number of streams that need to be changed.

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
