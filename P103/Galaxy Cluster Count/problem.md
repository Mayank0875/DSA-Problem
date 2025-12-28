## Title
Galaxy Cluster Count

## Slug
galaxy-cluster-count

## Difficulty
Medium

## Description
An astronomer analyzes a deep-space scan. The grid represents a sector of the universe where '1' is a star system and '0' is empty void. Stars close together form a galaxy.

You are given a star map represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents star system.
* `'0'` represents void.

A **galaxy** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by void beyond its boundaries.

Your task is to determine the total number of distinct galaxies in the star map.

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
All star system cells are connected, forming a single large galaxy.

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
There are three separate galaxies:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of galaxies.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
