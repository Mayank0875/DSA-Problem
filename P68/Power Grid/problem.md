## Title
Power Grid

## Slug
power-grid

## Difficulty
Hard

## Description
n power stations are distributed across a region. Transmission lines connect them into grids. A grid is stable if the number of stations is a 'Watt Number' (digits 4 and 7).

Engineers can build new lines. Merging k grids requires k - 1 new lines.

Your task is to determine the minimum number of extra lines the engineer needs to build to create at least one grid whose size is a Watt Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect station 4 with station 3. We can also connect 4 with 1 or 2. This creates a grid of size 4 (a Watt Number).

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
There is no way to connect the stations to form a grid with a size equal to a Watt Number.

## Input Format
- The first line contains two integers n and m: the number of stations and the number of existing lines.
- The next m lines each contain two integers u and v, representing a line between station u and station v. Note that u may be equal to v, and there may be multiple lines connecting the same pair of stations.

## Output Format
- Return a single integer: the minimum number of lines to build. If no solution exists, print -1.

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
