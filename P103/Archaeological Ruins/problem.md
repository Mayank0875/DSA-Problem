## Title
Archaeological Ruins

## Slug
archaeological-ruins

## Difficulty
Medium

## Description
A LIDAR scan reveals buried structures. '1' is a stone foundation and '0' is soil. Connected stones form a building ruin.

You are given a LIDAR scan represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents stone.
* `'0'` represents soil.

A **ruin** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by soil beyond its boundaries.

Your task is to determine the total number of distinct ruins in the LIDAR scan.

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
All stone cells are connected, forming a single large ruin.

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
There are three separate ruins:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of ruins.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
