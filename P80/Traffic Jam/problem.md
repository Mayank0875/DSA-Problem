## Title
Traffic Jam

## Slug
traffic-jam

## Difficulty
Medium

## Description
Cars flood from the Stadium (node 1) to the Bridge (node n).

The city roads consists of $n$ intersections connected by $m$ two-way lanes.
The traffic is attempting to travel from the Stadium (node 1) to the Bridge (node $n$).

To prevent this, you can close specific lanes. Closing a lane stops the flow.

Your task is to calculate the **minimum number of lanes** that must be closed to completely sever all routes between the Stadium and the Bridge.

## Examples

### 1

#### Input
4 5
1 2
1 3
2 3
3 4
1 4

#### Output
2

#### Explanation
The minimum is 2.

### 2

#### Input
3 3
1 2
2 3
1 3

#### Output
2

#### Explanation
We can close edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of intersections and lanes.
- The next $m$ lines describe the lanes. Each line contains two integers $a$ and $b$, indicating a lane between intersection $a$ and intersection $b$.

## Output Format
- Return one integer: the minimum number of lanes that need to be closed.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
