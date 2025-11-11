## Title

Data Rift: Packing Data Blocks

## Slug

data-rift-packing-data-blocks

## Difficulty

Medium

## Description

In the Data Rift, engineers must store a massive number of identical data blocks inside a square memory sector.  
Each block occupies a rectangle w units wide and h units tall, and blocks cannot be rotated.  
Given n such blocks, determine the smallest possible side length of a square sector that can contain all n blocks without overlap.  

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits floor(9/2) = 4 blocks across and floor(9/3) = 3 blocks down, giving 4 × 3 = 12 blocks — enough for 10.  
A square of side 8 fits floor(8/2) × floor(8/3) = 4 × 2 = 8 blocks — not enough.  
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits floor(2/1) × floor(2/1) = 2 × 2 = 4 blocks.  
A square of side 1 fits only 1 × 1 = 1 block.  
Therefore, the minimum side length needed for 3 blocks is 2.
  
## Input Format  

- Three space-separated integers w, h, and n.

## Output Format  

- Return single integer representing the minimum side length of the square sector.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory