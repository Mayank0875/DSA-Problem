## Title

Reconstructing the Shattered Spectrum

## Slug

shattered-spectrum

## Difficulty

Medium

## Description

The ancient crystal of the Shattered Spectrum has broken into many rectangular shards. There are **n** identical shards, each **w** units wide and **h** units long. To restore the crystal, all shards must be placed flat inside a single square containment field. The shards cannot be rotated. Determine the smallest possible side length of the square field that can hold all **n** shards without overlap.

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits floor(9/2) = 4 shards across and floor(9/3) = 3 shards down, giving 4 × 3 = 12 shards — enough for 10.  
A square of side 8 fits floor(8/2) × floor(8/3) = 4 × 2 = 8 shards — not enough.  
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits floor(2/1) × floor(2/1) = 2 × 2 = 4 shards.  
A square of side 1 fits only 1 × 1 = 1 shard.  
Therefore, the minimum side length needed for 3 shards is 2.
  
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