## Title
Network Outage

## Slug
network-outage

## Difficulty
Medium

## Description
A network monitor shows server status. '1' is a down server and '0' is active. Connected down servers indicate a regional failure cluster.

You are given a network grid represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents offline server.
* `'0'` represents online server.

A **failure cluster** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by online server beyond its boundaries.

Your task is to determine the total number of distinct failure clusters in the network grid.

## Examples

### 1

#### Input
4 5
1 1 1 1 0
1 1 0 1 0
1 1 0 0 0
0 0 0 0 0

#### Output
1

#### Explanation
All offline server cells are connected, forming a single large failure cluster.

### 2

#### Input
4 5
1 1 0 0 0
1 1 0 0 0
0 0 1 0 0
0 0 0 1 1

#### Output
3

#### Explanation
There are three separate failure clusters:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of failure clusters.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
