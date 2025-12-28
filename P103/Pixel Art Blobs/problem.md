## Title
Pixel Art Blobs

## Slug
pixel-art-blobs

## Difficulty
Medium

## Description
An image processing algorithm analyzes a black and white image. '1' is a black pixel, '0' is white. Count the number of connected black shapes (blobs).

You are given a image bitmap represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents black pixel.
* `'0'` represents white pixel.

A **shape** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by white pixel beyond its boundaries.

Your task is to determine the total number of distinct shapes in the image bitmap.

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
All black pixel cells are connected, forming a single large shape.

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
There are three separate shapes:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of shapes.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
