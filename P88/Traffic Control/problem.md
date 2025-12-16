## Title
Traffic Control

## Slug
traffic-control

## Difficulty
Medium

## Description
Roads feeding an intersection have different traffic flows. The light turns green only if the waiting cars on a set of roads represent the majority of total traffic.

Your task is to count the number of **traffic patternss**. A traffic pattern is considered valid if it satisfies two specific criteria:
1.  **Green Light:** The total traffic flow of the traffic pattern is strictly greater than half of the total traffic flow across all roads.
2.  **No Superfluous roads:** The traffic pattern is minimal. This means that removing **any one** road from the traffic pattern would cause the remaining total to drop to half or less of the total traffic flow (losing the Green Light).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total traffic flow is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total traffic flow = 10. Half = 5.
Valid traffic patternss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of roads.
- The second line contains n integers: the traffic flow of each road.

## Output Format
- Return one integer: the total number of valid traffic patternss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ traffic flow ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
