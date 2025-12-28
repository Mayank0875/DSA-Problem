## Title
Oil Spill Containment

## Slug
oil-spill-containment

## Difficulty
Medium

## Description
An environmental agency tracks an oil spill. '1' represents oil slick and '0' represents clean water. They need to count the number of separate slicks to deploy containment booms.

You are given a ocean scan represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents oil.
* `'0'` represents clean water.

A **slick** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by clean water beyond its boundaries.

Your task is to determine the total number of distinct slicks in the ocean scan.

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
All oil cells are connected, forming a single large slick.

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
There are three separate slicks:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of slicks.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
