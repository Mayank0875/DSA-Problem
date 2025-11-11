## Title

Parallel Labyrinth

## Slug

parallel-labyrinth

## Difficulty

Medium

## Description

The ancient maze is being expanded with n identical rectangular chambers.  
Each chamber is w units wide and h units long. To keep the maze compact, all chambers must be placed flat inside a single square section of the labyrinth.  
Chambers cannot be rotated.  

Your task is to determine the smallest possible side length of a square that can accommodate all n chambers without any overlap.

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits ⌊9/2⌋ = 4 chambers across and ⌊9/3⌋ = 3 chambers down, giving 4 × 3 = 12 chambers — enough for 10.  
A square of side 8 fits ⌊8/2⌋ × ⌊8/3⌋ = 4 × 2 = 8 chambers — not enough.  
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits ⌊2/1⌋ × ⌊2/1⌋ = 2 × 2 = 4 chambers.  
A square of side 1 fits only 1 × 1 = 1 chamber.  
Therefore, the minimum side length needed for 3 chambers is 2.
  
## Input Format  

- Three space-separated integers w, h, and n.

## Output Format  

- Return single integer representing the minimum side length of the square section.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory