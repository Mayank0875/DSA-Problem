## Title
Glacier Meltwater

## Slug
glacier-meltwater

## Difficulty
Medium

## Description
Meltwater forms streams on ice. All water must flow into the Glacial Lake.

There are $n$ crevasses numbered from $1$ to $n$, connected by $n-1$ streams. The network forms a tree structure (there is exactly one path between any two crevasses). Currently, all streams are one-way.

Nature directs water to the **Glacial Lake (Node 1)**. To ensure success, every other crevasse must be able to reach Glacial Lake by traveling along the streams in the correct direction.

You are given the current orientation of the streams. Your task is to determine the **minimum** number of streams that need to be channeled so that every crevasse can reach Glacial Lake.

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
The destination is Glacial Lake (1).
- Stream 1->2 points away from 1. Needs channeling.
- Stream 2->4 points away from 1. Needs channeling.
- Stream 3->2 points towards 2 (and effectively towards 1). OK.
- Stream 5->1 points towards 1. OK.
- Stream 5->6 points away from 1 (via 5). Needs channeling.
Total channelings: 3.

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
Streams 2->3 and 4->5 need to be channeled.

## Input Format
- The first line contains an integer $n$ — the number of crevasses.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way stream from crevasse $u$ to crevasse $v$.

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
