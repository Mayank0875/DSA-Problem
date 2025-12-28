## Title
Iceberg Tracker

## Slug
iceberg-tracker

## Difficulty
Medium

## Description
A ship radar detects ice. '1' is ice and '0' is ocean. To navigate safely, the captain needs the count of distinct icebergs.

You are given a radar screen represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents ice.
* `'0'` represents ocean.

A **iceberg** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by ocean beyond its boundaries.

Your task is to determine the total number of distinct icebergs in the radar screen.

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
All ice cells are connected, forming a single large iceberg.

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
There are three separate icebergs:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of icebergs.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
