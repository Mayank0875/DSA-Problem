## Title

Infinite Loopstorm: Packing Rectangular Loops

## Slug

infinite-loopstorm-packing-rectangular-loops

## Difficulty

Medium

## Description

During the legendary Infinite Loopstorm, the storm‑weavers must store a massive number of rectangular loops inside a single square vortex.  
There are **n** identical loops, each having a width of **w** units and a height of **h** units. The loops cannot be rotated; they must be placed axis‑aligned.  
Your mission is to determine the smallest possible side length of a square vortex that can contain all **n** loops without any overlap.  

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits floor(9/2) = 4 loops across and floor(9/3) = 3 loops down, giving 4 × 3 = 12 loops — enough for 10.  
A square of side 8 fits floor(8/2) × floor(8/3) = 4 × 2 = 8 loops — not enough.  
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits floor(2/1) × floor(2/1) = 2 × 2 = 4 loops.  
A square of side 1 fits only 1 × 1 = 1 loop.  
Therefore, the minimum side length needed for 3 loops is 2.
  
## Input Format  

- Three space-separated integers w, h, and n.

## Output Format  

- Return single integer representing the minimum side length of the square vortex.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory