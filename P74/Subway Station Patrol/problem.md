## Title
Subway Station Patrol

## Slug
subway-station-patrol

## Difficulty
Medium

## Description
Stations are connected by tunnels. Police officers stationed at stops need to partner up with an officer at an adjacent station for patrols.

The structure is a tree with n stations and n-1 tunnels.
A patrol unit is formed between two stations connected by a tunnel.
However, each station can be part of at most one patrol unit.

Your task is to calculate the maximum number of patrol units that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of patrol units is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 patrol units.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form patrol units (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of stations.
- The next n-1 lines each contain two integers u and v, representing a tunnel between station u and station v.

## Output Format
- Return a single integer representing the maximum number of patrol units.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
