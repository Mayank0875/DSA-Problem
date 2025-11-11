## Title

Phantom Recursion: Minimal Square for Spectral Tiles

## Slug

phantom-recursion

## Difficulty

Medium

## Description

A phantom programmer is conjuring a square arena to trap n identical spectral tiles.  
Each tile is w units wide and h units long, and the tiles must remain oriented as given (no rotation).  
The goal is to find the smallest possible side length of a square arena that can hold all n tiles flat without any overlap.

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits floor(9/2) = 4 tiles across and floor(9/3) = 3 tiles down, giving 4 × 3 = 12 tiles — enough for 10.  
A square of side 8 fits floor(8/2) × floor(8/3) = 4 × 2 = 8 tiles — not enough.  
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits floor(2/1) × floor(2/1) = 2 × 2 = 4 tiles.  
A square of side 1 fits only 1 × 1 = 1 tile.  
Therefore, the minimum side length needed for 3 tiles is 2.
  
## Input Format  

- Three space-separated integers w, h, and n.

## Output Format  

- Return single integer representing the minimum side length of the square arena.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory