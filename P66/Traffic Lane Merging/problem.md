## Title
Traffic Lane Merging

## Slug
traffic-lane-merging

## Difficulty
Medium

## Description
Two highway lanes need merge points to allow flow if a lane is blocked.

Two parallel lanes, Lane 1 and Lane 2, each contain n segments arranged in a line.
Lane 1 has an array `a` representing the speed limit of each segment.
Lane 2 has an array `b` representing the speed limit of each segment.

Inside each lane, adjacent segments are already connected by internal road.

You must establish inter-lane merge paths connecting some segments of Lane 1 to some segments of Lane 2.

The cost to create a path between segment i of Lane 1 and segment j of Lane 2 is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single segment is removed (from either Lane 1 or Lane 2).
If one segment fails and disappears along with all its connections, the remaining segments must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of segments:
1. segment 1 from Lane 1 with segment 2 from Lane 2: cost |1-4| = 3.
2. segment 3 from Lane 1 with segment 2 from Lane 2: cost |1-4| = 3.
3. segment 2 from Lane 1 with segment 1 from Lane 2: cost |10-20| = 10.
4. segment 2 from Lane 1 with segment 3 from Lane 2: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first segment of Lane 1 with the first of Lane 2, and the last segment of Lane 1 with the last of Lane 2, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of segments in each lane.
- The second line contains n integers representing the speed limits of Lane 1.
- The third line contains n integers representing the speed limits of Lane 2.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
