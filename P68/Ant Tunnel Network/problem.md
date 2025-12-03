## Title
Ant Tunnel Network

## Slug
ant-tunnel-network

## Difficulty
Hard

## Description
An ant hill has n chambers. Pheromone trails connect some. The Queen prefers sections with a 'Royal Count' of chambers (digits 4 and 7).

Worker ants can dig new trails. Merging k sections costs k - 1 trails.

Your task is to determine the minimum number of extra trails the Queen needs to build to create at least one section whose size is a Royal Count. If this goal cannot be achieved, return -1.

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
The optimal way is to connect chamber 4 with chamber 3. We can also connect 4 with 1 or 2. This creates a section of size 4 (a Royal Count).

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
There is no way to connect the chambers to form a section with a size equal to a Royal Count.

## Input Format
- The first line contains two integers n and m: the number of chambers and the number of existing trails.
- The next m lines each contain two integers u and v, representing a trail between chamber u and chamber v. Note that u may be equal to v, and there may be multiple trails connecting the same pair of chambers.

## Output Format
- Return a single integer: the minimum number of trails to build. If no solution exists, print -1.

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
