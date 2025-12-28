## Title
Rust Spots

## Slug
rust-spots

## Difficulty
Medium

## Description
A mechanic inspects a car chassis. '1' is a rust spot and '0' is clean metal. Connected spots form a rusted area.

You are given a metal surface represented by an $m \times n$ 2D binary grid called `grid`.
In this grid:
* `'1'` represents rust.
* `'0'` represents metal.

A **rusted area** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by metal beyond its boundaries.

Your task is to determine the total number of distinct rusted areas in the metal surface.

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
All rust cells are connected, forming a single large rusted area.

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
There are three separate rusted areas:
1. Top-left corner.
2. The single cell in the middle.
3. Bottom-right corner.

## Input Format
- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the grid.

## Output Format
- Return a single integer representing the number of rusted areas.

## Constraints
- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, depth-first-search, graph
