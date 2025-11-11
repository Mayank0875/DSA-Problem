## Title

Digital Mirage: Arranging Rectangular Panels

## Slug

digital-mirage-arrangement

## Difficulty

Medium

## Description

In the virtual realm of Digital Mirage, designers need to arrange n identical rectangular holographic panels inside a single square projection area.  
Each panel has a width of w units and a height of h units. The panels must be placed flat and cannot be rotated.  
Your task is to determine the smallest possible side length of a square projection that can contain all n panels without overlap.

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits floor(9/2) = 4 panels across and floor(9/3) = 3 panels down, giving 4 × 3 = 12 panels — enough for 10.  
A square of side 8 fits floor(8/2) × floor(8/3) = 4 × 2 = 8 panels — not enough.  
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits floor(2/1) × floor(2/1) = 2 × 2 = 4 panels.  
A square of side 1 fits only 1 × 1 = 1 panel.  
Therefore, the minimum side length needed for 3 panels is 2.
  
## Input Format  

- Three space-separated integers w, h, and n.

## Output Format  

- Return single integer representing the minimum side length of the square container.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory