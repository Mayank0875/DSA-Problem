## Title
Railway Network

## Slug
railway-network

## Difficulty
Hard

## Description
n cities have some railway tracks connecting them. The Minister of Transport wants a connected region with a 'Lucky Population' of cities (digits 4 and 7).

New tracks can be laid. Merging k regions requires laying k - 1 new tracks.

Your task is to determine the minimum number of extra tracks the Minister needs to build to create at least one region whose size is a Lucky Population. If this goal cannot be achieved, return -1.

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
The optimal way is to connect city 4 with city 3. We can also connect 4 with 1 or 2. This creates a region of size 4 (a Lucky Population).

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
There is no way to connect the cities to form a region with a size equal to a Lucky Population.

## Input Format
- The first line contains two integers n and m: the number of cities and the number of existing tracks.
- The next m lines each contain two integers u and v, representing a track between city u and city v. Note that u may be equal to v, and there may be multiple tracks connecting the same pair of cities.

## Output Format
- Return a single integer: the minimum number of tracks to build. If no solution exists, print -1.

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
