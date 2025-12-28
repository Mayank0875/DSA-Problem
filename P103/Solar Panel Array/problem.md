## Title
Solar Panel Array

## Slug
solar-panel-array

## Difficulty
Medium

## Description
A maintenance drone checks a solar farm. '1' is a functioning panel and '0' is a broken one (or gap). Wait, actually let's count broken clusters. '1' is broken, '0' is working.

You are given a array grid represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents broken panel.
* `'0'` represents working panel.

A **damage cluster** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by working panel beyond its boundaries.

Your task is to determine the total number of distinct damage clusters in the array grid.

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
All broken panel cells are connected, forming a single large damage cluster.

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
There are three separate damage clusters:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of damage clusters.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
