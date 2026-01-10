## Title
Nerve Impulses

## Slug
nerve-impulses

## Difficulty
Medium

## Description
A neurologist studies reflexes. Sensory signals must travel to the Brain Stem.

There are $n$ ganglia numbered from $1$ to $n$, connected by $n-1$ axons. The network forms a tree structure (there is exactly one path between any two ganglia). Currently, all axons are one-way.

The nervous system transmits to the **Brain Stem (Node 1)**. To ensure success, every other ganglion must be able to reach Brain Stem by traveling along the axons in the correct direction.

You are given the current orientation of the axons. Your task is to determine the **minimum** number of axons that need to be corrected so that every ganglion can reach Brain Stem.

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
The destination is Brain Stem (1).
- Axon 1->2 points away from 1. Needs correction.
- Axon 2->4 points away from 1. Needs correction.
- Axon 3->2 points towards 2 (and effectively towards 1). OK.
- Axon 5->1 points towards 1. OK.
- Axon 5->6 points away from 1 (via 5). Needs correction.
Total corrections: 3.

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
Axons 2->3 and 4->5 need to be corrected.

## Input Format
- The first line contains an integer $n$ — the number of ganglia.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way axon from ganglion $u$ to ganglion $v$.

## Output Format
- Return a single integer representing the minimum number of axons that need to be changed.

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
