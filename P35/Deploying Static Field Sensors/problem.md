## Title

Deploying Static Field Sensors

## Slug

static-field

## Difficulty

Medium

## Description

A research team is setting up a static electromagnetic field using rectangular sensor panels. They have n identical panels, each w units wide and h units long. All panels must be placed flat on a square field without overlapping and cannot be rotated. Determine the smallest possible side length of the square field that can accommodate all n panels.

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