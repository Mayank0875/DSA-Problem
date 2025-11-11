## Title

Harmonic Matrix

## Slug

harmonic-matrix

## Difficulty

Medium

## Description

A composer arranges n harmonic tones in a row, numbered 1 to n. Initially, all tones are resonating.
The composer performs n harmonic operations. For the i‑th operation (where i goes from 1 to n), every tone whose number j is a multiple of i flips its state. 
A resonating tone becomes silent, and a silent tone becomes resonating. After all n operations are applied, the composer observes the final state of the tones. The composer needs exactly k tones to be resonating in the end. Find the smallest possible number of tones n the composer should start with to achieve exactly k resonating tones.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [R]. Operation 1 flips 1: [S]. Final: 0 resonating.
If n=2, initial: [R, R]. Operation 1 flips 1, 2: [S, S]. Operation 2 flips 2: [S, R]. Final: 1 resonating (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [R,R,R,R,R].
Operation 1 flips 1,2,3,4,5 -> [S,S,S,S,S].
Operation 2 flips 2,4 -> [S,R,S,R,S].
Operation 3 flips 3 -> [S,R,R,R,S].
Operation 4 flips 4 -> [S,R,R,S,S].
Operation 5 flips 5 -> [S,R,R,S,R].
Final state: 3 tones (2, 3, 5) are resonating (k=3). We can show n=4 results in only 2 resonating tones ([S,R,R,S]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of tones required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory