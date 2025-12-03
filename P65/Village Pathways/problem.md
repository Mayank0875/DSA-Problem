## Title
Village Pathways

## Slug
village-pathways

## Difficulty
Medium

## Description
Houses are connected by paths. A Neighborhood is a group of houses mutually reachable.

Two houses a and b belong to the same Neighborhood if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of paths.
In other words, two houses are in the same Neighborhood if they are mutually reachable.

Your task is to: Determine how many Neighborhoods exist in total.

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
The houses form two distinct groups where round-trip traversal is possible within each group.
Houses {1, 2, 3} form one Neighborhood.
Path: 1 -> 2 -> 3 -> 1.
Houses {4, 5} form another Neighborhood.
Path: 4 -> 5 -> 4.
Total Neighborhoods: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 houses and 1 one-way path.
Path: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Neighborhoods.

## Input Format
- The first line contains two integers n and m: the number of houses and paths.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way path from house a to house b.

## Output Format
- Return one integer: the total number of Neighborhoods.

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
