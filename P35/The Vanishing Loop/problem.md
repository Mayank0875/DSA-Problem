## Title

The Vanishing Loop

## Slug

the-vanishing-loop

## Difficulty

Medium

## Description

A mischievous sorcerer has summoned **n** identical rectangular loops that appear on the ground.  
Each loop occupies a rectangle of width **w** units and height **h** units.  
Before the loops vanish, they must all be placed flat inside a single square arena.  
The loops cannot be rotated.  

Your task is to determine the smallest possible side length of a square arena that can hold all **n** loops without any overlap.

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

- Return single integer representing the minimum side length of the square arena.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory