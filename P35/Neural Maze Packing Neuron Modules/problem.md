## Title

Neural Maze: Packing Neuron Modules

## Slug

neural-maze

## Difficulty

Medium

## Description

In a cutting‑edge neural‑chip design, engineers need to embed n identical rectangular neuron modules onto a square silicon substrate.  
Each module occupies a rectangle of width w units and height h units. The modules must be placed flat, aligned with the substrate axes, and cannot be rotated.  

Your task is to determine the smallest possible side length of a square substrate that can accommodate all n modules without overlap.

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits floor(9/2) = 4 modules across and floor(9/3) = 3 modules down, giving 4 × 3 = 12 modules — enough for 10.  
A square of side 8 fits floor(8/2) × floor(8/3) = 4 × 2 = 8 modules — not enough.  
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits floor(2/1) × floor(2/1) = 2 × 2 = 4 modules.  
A square of side 1 fits only 1 × 1 = 1 module.  
Therefore, the minimum side length needed for 3 modules is 2.
  
## Input Format  

- Three space-separated integers w, h, and n.

## Output Format  

- Return single integer representing the minimum side length of the square substrate.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory