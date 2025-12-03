## Title
Traffic Grid

## Slug
traffic-grid

## Difficulty
Hard

## Description
n intersections are in a city. Streets connect some into districts. Planners want districts of 'Flow Number' (digits 4 and 7).

You can build streets. Merging k districts requires k - 1 new streets.

Your task is to determine the minimum number of extra streets the planner needs to build to create at least one district whose size is a Flow Number. If this goal cannot be achieved, return -1.

## Examples

### 1

#### Input
4 3
1 2
2 3
1 3

#### Output
1

#### Explanation
The optimal way is to connect intersection 4 with intersection 3. We can also connect 4 with 1 or 2. This creates a district of size 4 (a Flow Number).

### 2

#### Input
5 4
1 2
3 4
4 5
3 5

#### Output
-1

#### Explanation
There is no way to connect the intersections to form a district with a size equal to a Flow Number.

## Input Format
- The first line contains two integers n and m: the number of intersections and the number of existing streets.
- The next m lines each contain two integers u and v, representing a street between intersection u and intersection v. Note that u may be equal to v, and there may be multiple streets connecting the same pair of intersections.

## Output Format
- Return a single integer: the minimum number of streets to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
