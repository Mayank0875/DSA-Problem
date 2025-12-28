## Title
Rooftop Gardens

## Slug
rooftop-gardens

## Difficulty
Medium

## Description
A city planner reviews aerial footage. '1' represents a green roof garden and '0' is concrete. Count the number of distinct green spaces.

You are given a city map represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents garden.
* `'0'` represents concrete.

A **green space** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by concrete beyond its boundaries.

Your task is to determine the total number of distinct green spaces in the city map.

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
All garden cells are connected, forming a single large green space.

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
There are three separate green spaces:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of green spaces.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
