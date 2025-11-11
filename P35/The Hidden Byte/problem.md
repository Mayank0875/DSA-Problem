## Title

The Hidden Byte

## Slug

the-hidden-byte

## Difficulty

Medium

## Description

A secretive programmer is trying to hide n identical data blocks in a memory cache.  
Each block occupies a rectangle that is w bytes wide and h bytes tall.  
To keep the cache compact, all blocks must be placed flat inside a single square memory region.  
The blocks cannot be rotated.  
Your task is to determine the minimum possible side length of the square region that can contain all n blocks without any overlap.

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

- Return single integer representing the minimum side length of the square container.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory