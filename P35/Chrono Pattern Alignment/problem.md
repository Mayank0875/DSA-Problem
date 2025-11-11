## Title

Chrono Pattern Alignment

## Slug

chrono-pattern

## Difficulty

Medium

## Description

The Chronomancers are arranging identical temporal shards on a time‑grid.  
Each shard occupies a rectangle of width **w** time‑units and height **h** time‑units.  
To stabilize the Chrono Pattern, all **n** shards must be placed flat inside a single square time‑field.  
The shards cannot be rotated. Your task is to determine the smallest possible side length of the square time‑field that can contain all **n** shards without overlap.

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

- Return single integer representing the minimum side length of the square container.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory