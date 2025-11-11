## Title

The Obsidian Key

## Slug

obsidian-key

## Difficulty

Medium

## Description

The ancient Obsidian Key has been shattered into n identical rectangular fragments, each w units wide and h units long. To restore the key, a master artisan must place all fragments flat inside a single square vault. The fragments cannot be rotated. Your task is to determine the smallest possible side length of the square vault that can accommodate all n fragments without overlap.

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits floor(9/2) = 4 fragments across and floor(9/3) = 3 fragments down, giving 4 × 3 = 12 fragments — enough for 10.
A square of side 8 fits floor(8/2) × floor(8/3) = 4 × 2 = 8 fragments — not enough.
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits floor(2/1) × floor(2/1) = 2 × 2 = 4 fragments.
A square of side 1 fits only 1 × 1 = 1 fragment.
Therefore, the minimum side length needed for 3 fragments is 2.
  
## Input Format  

- Three space-separated integers w, h, and n.

## Output Format  

- Return single integer representing the minimum side length of the square vault.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory