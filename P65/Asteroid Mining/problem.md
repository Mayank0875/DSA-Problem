## Title
Asteroid Mining

## Slug
asteroid-mining

## Difficulty
Medium

## Description
Miners travel between asteroids. A Mining Sector is a group of asteroids mutually reachable.

Two asteroids a and b belong to the same Sector if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of shuttles.
In other words, two asteroids are in the same Sector if they are mutually reachable.

Your task is to: Determine how many Sectors exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The asteroids form two distinct groups where round-trip traversal is possible within each group.
Asteroids {1, 2, 3} form one Sector.
Path: 1 -> 2 -> 3 -> 1.
Asteroids {4, 5} form another Sector.
Path: 4 -> 5 -> 4.
Total Sectors: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 asteroids and 1 one-way shuttle.
Shuttle: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Sectors.

## Input Format
- The first line contains two integers n and m: the number of asteroids and shuttles.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way shuttle from asteroid a to asteroid b.

## Output Format
- Return one integer: the total number of Sectors.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, strongly-connected-components
