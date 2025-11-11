## Title

Code Abyss: Packing Rectangular Modules

## Slug

code-abyss-packing-rectangular-modules

## Difficulty

Medium

## Description

In the depths of the Code Abyss, developers are preparing to deploy a massive batch of identical rectangular code modules. Each module occupies **w** units in width and **h** units in height. To ship them safely, they must be placed flat inside a single square deployment container. The modules cannot be rotated. Your task is to help the developers find the side length of the smallest possible square container that can hold all **n** modules without any overlap.

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits floor(9/2) = 4 boxes across and floor(9/3) = 3 boxes down, giving 4 × 3 = 12 boxes — enough for 10.
A square of side 8 fits floor(8/2) × floor(8/3) = 4 × 2 = 8 boxes — not enough.
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits floor(2/1) × floor(2/1) = 2 × 2 = 4 boxes.
A square of side 1 fits only 1 × 1 = 1 box.
Therefore, the minimum side length needed for 3 boxes is 2.
  
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