## Title
Lava Flow

## Slug
lava-flow

## Difficulty
Medium

## Description
A volcano erupts. Lava channels flow down to the Sea.

There are $n$ craters numbered from $1$ to $n$, connected by $n-1$ channels. The network forms a tree structure (there is exactly one path between any two craters). Currently, all channels are one-way.

Gravity pulls the molten rock to the **Sea (Node 1)**. To ensure success, every other crater must be able to reach Sea by traveling along the channels in the correct direction.

You are given the current orientation of the channels. Your task is to determine the **minimum** number of channels that need to be diverted so that every crater can reach Sea.

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
The destination is Sea (1).
- Channel 1->2 points away from 1. Needs diversion.
- Channel 2->4 points away from 1. Needs diversion.
- Channel 3->2 points towards 2 (and effectively towards 1). OK.
- Channel 5->1 points towards 1. OK.
- Channel 5->6 points away from 1 (via 5). Needs diversion.
Total diversions: 3.

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
Channels 2->3 and 4->5 need to be diverted.

## Input Format
- The first line contains an integer $n$ — the number of craters.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way channel from crater $u$ to crater $v$.

## Output Format
- Return a single integer representing the minimum number of channels that need to be changed.

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
