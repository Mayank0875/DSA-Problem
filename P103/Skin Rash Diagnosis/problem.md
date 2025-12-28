## Title
Skin Rash Diagnosis

## Slug
skin-rash-diagnosis

## Difficulty
Medium

## Description
A dermatologist scans skin. '1' is inflamed skin, '0' is healthy. Connected inflamed points form a rash patch.

You are given a skin scan represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents inflammation.
* `'0'` represents healthy skin.

A **rash** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by healthy skin beyond its boundaries.

Your task is to determine the total number of distinct rashes in the skin scan.

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
All inflammation cells are connected, forming a single large rash.

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
There are three separate rashes:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of rashes.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
