## Title
Gold Veins

## Slug
gold-veins

## Difficulty
Medium

## Description
A geological survey shows rock composition. '1' is gold ore, '0' is granite. Connected ore blocks form a gold vein.

You are given a rock layer represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents ore.
* `'0'` represents granite.

A **vein** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by granite beyond its boundaries.

Your task is to determine the total number of distinct veins in the rock layer.

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
All ore cells are connected, forming a single large vein.

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
There are three separate veins:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of veins.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
