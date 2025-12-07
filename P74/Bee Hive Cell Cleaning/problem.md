## Title
Bee Hive Cell Cleaning

## Slug
bee-hive-cell-cleaning

## Difficulty
Medium

## Description
Bees are cleaning honeycomb cells. Two bees in adjacent cells can work together to clean the wall between them. Each bee helps with one wall.

The structure is a tree with n cells and n-1 walls.
A cleaning team is formed between two cells connected by a wall.
However, each cell can be part of at most one cleaning team.

Your task is to calculate the maximum number of cleaning teams that can be formed.

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
One optimal set of cleaning teams is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 cleaning teams.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form cleaning teams (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of cells.
- The next n-1 lines each contain two integers u and v, representing a wall between cell u and cell v.

## Output Format
- Return a single integer representing the maximum number of cleaning teams.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
