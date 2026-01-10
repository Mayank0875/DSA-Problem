## Title
Water Slide Park

## Slug
water-slide-park

## Difficulty
Medium

## Description
Kids slide down tubes. All tubes must end at the Splash Pool.

There are $n$ platforms numbered from $1$ to $n$, connected by $n-1$ slides. The network forms a tree structure (there is exactly one path between any two platforms). Currently, all slides are one-way.

Gravity pulls riders to the **Splash Pool (Node 1)**. To ensure success, every other platform must be able to reach Splash Pool by traveling along the slides in the correct direction.

You are given the current orientation of the slides. Your task is to determine the **minimum** number of slides that need to be re-routed so that every platform can reach Splash Pool.

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
The destination is Splash Pool (1).
- Slide 1->2 points away from 1. Needs re-routing.
- Slide 2->4 points away from 1. Needs re-routing.
- Slide 3->2 points towards 2 (and effectively towards 1). OK.
- Slide 5->1 points towards 1. OK.
- Slide 5->6 points away from 1 (via 5). Needs re-routing.
Total re-routings: 3.

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
Slides 2->3 and 4->5 need to be re-routed.

## Input Format
- The first line contains an integer $n$ — the number of platforms.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way slide from platform $u$ to platform $v$.

## Output Format
- Return a single integer representing the minimum number of slides that need to be changed.

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
