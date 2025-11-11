## Title

Shadow Spectrum

## Slug

shadow-spectrum

## Difficulty

Medium

## Description

A sorcerer arranges n spectral shadows in a row, numbered 1 to n. Initially, all shadows are bright.
The sorcerer performs n incantations. For the i‑th incantation (where i goes from 1 to n), every shadow whose number j is a multiple of i flips its state. 
A bright shadow becomes dim, and a dim shadow becomes bright. After all n incantations are cast, the sorcerer observes the final state of the shadows. The sorcerer needs exactly k shadows to be bright in the end. Find the smallest possible number of shadows n the sorcerer should start with to achieve exactly k bright shadows.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [B]. Incantation 1 flips 1: [D]. Final: 0 bright.
If n=2, initial: [B, B]. Incantation 1 flips 1, 2: [D, D]. Incantation 2 flips 2: [D, B]. Final: 1 bright (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [B,B,B,B,B].
Incantation 1 flips 1,2,3,4,5 -> [D,D,D,D,D].
Incantation 2 flips 2,4 -> [D,B,D,B,D].
Incantation 3 flips 3 -> [D,B,B,B,D].
Incantation 4 flips 4 -> [D,B,B,D,D].
Incantation 5 flips 5 -> [D,B,B,D,B].
Final state: 3 shadows (2, 3, 5) are bright (k=3). We can show n=4 results in only 2 bright shadows ([D,B,B,D]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of shadows required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory