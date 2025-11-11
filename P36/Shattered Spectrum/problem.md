## Title

Shattered Spectrum

## Slug

shattered-spectrum

## Difficulty

Medium

## Description

A light engineer arranges n color filters in a row, numbered 1 to n. Initially, all filters are transmitting light (bright).
The engineer performs n adjustments. For the i‑th adjustment (where i goes from 1 to n), every filter whose number j is a multiple of i flips its state. 
A bright filter becomes dim, and a dim filter becomes bright. After all n adjustments are applied, the engineer observes the final state of the filters. The engineer needs exactly k filters to be bright in the end. Find the smallest possible number of filters n the engineer should start with to achieve exactly k bright filters.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [B]. Adjustment 1 flips 1: [D]. Final: 0 bright.
If n=2, initial: [B, B]. Adjustment 1 flips 1, 2: [D, D]. Adjustment 2 flips 2: [D, B]. Final: 1 bright (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [B,B,B,B,B].
Adjustment 1 flips 1,2,3,4,5 -> [D,D,D,D,D].
Adjustment 2 flips 2,4 -> [D,B,D,B,D].
Adjustment 3 flips 3 -> [D,B,B,B,D].
Adjustment 4 flips 4 -> [D,B,B,D,D].
Adjustment 5 flips 5 -> [D,B,B,D,B].
Final state: 3 filters (2, 3, 5) are bright (k=3). We can show n=4 results in only 2 bright filters ([D,B,B,D]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of filters required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory