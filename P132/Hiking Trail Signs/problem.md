## Title
Hiking Trail Signs

## Slug
hiking-trail-signs

## Difficulty
Medium

## Description
Hikers get lost easily. All trail signs must point towards the Visitor Center.

There are $n$ junctions numbered from $1$ to $n$, connected by $n-1$ trails. The network forms a tree structure (there is exactly one path between any two junctions). Currently, all trails are one-way.

Safety requires signs to lead to the **Visitor Center (Node 1)**. To ensure success, every other junction must be able to reach Visitor Center by traveling along the trails in the correct direction.

You are given the current orientation of the trails. Your task is to determine the **minimum** number of trails that need to be flipped so that every junction can reach Visitor Center.

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
The destination is Visitor Center (1).
- Trail 1->2 points away from 1. Needs flip.
- Trail 2->4 points away from 1. Needs flip.
- Trail 3->2 points towards 2 (and effectively towards 1). OK.
- Trail 5->1 points towards 1. OK.
- Trail 5->6 points away from 1 (via 5). Needs flip.
Total flips: 3.

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
Trails 2->3 and 4->5 need to be flipped.

## Input Format
- The first line contains an integer $n$ — the number of junctions.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way trail from junction $u$ to junction $v$.

## Output Format
- Return a single integer representing the minimum number of trails that need to be changed.

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
