## Title

The Archipelago Census

## Slug

the-archipelago-census

## Difficulty

Medium

## Description

The Navy has dispatched you to uncharted waters to map out a newly discovered archipelago. You are given a satellite map represented by an $m \times n$ 2D binary grid called `grid`.

In this map:
* `'1'` represents land.
* `'0'` represents water.

An **island** is defined as a contiguous group of `'1'`s connected horizontally or vertically (not diagonally). You may assume that the entire grid is surrounded by water beyond its boundaries.

Your task is to determine the total number of distinct islands in the archipelago so the Navy can update their charts.

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

All land masses are connected either horizontally or vertically, forming a single large island.
    
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

There are three separate clusters of land:
1. Top-left corner.
2. The single land cell in the middle.
3. Bottom-right corner.
  

## Input Format  

- The first line contains two integers `m` and `n`, representing the number of rows and columns.
- The next `m` lines contain `n` space-separated characters (`'0'` or `'1'`), representing the rows of the grid.

## Output Format  

- Return a single integer representing the number of islands.
  

## Constraints  

- 1 ≤ m, n ≤ 300
- `grid[i][j]` is `'0'` or `'1'`

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

breadth-first-search, depth-first-search, graph

## Company
ebay