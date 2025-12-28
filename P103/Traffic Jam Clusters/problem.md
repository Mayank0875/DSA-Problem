## Title
Traffic Jam Clusters

## Slug
traffic-jam-clusters

## Difficulty
Medium

## Description
A traffic grid shows congestion. '1' is a stopped car, '0' is moving traffic. Connected stopped cars form a traffic jam.

You are given a traffic grid represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents stopped car.
* `'0'` represents moving traffic.

A **traffic jam** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by moving traffic beyond its boundaries.

Your task is to determine the total number of distinct traffic jams in the traffic grid.

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
All stopped car cells are connected, forming a single large traffic jam.

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
There are three separate traffic jams:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of traffic jams.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
