## Title

Binary Ghost's Haunted Grid

## Slug

binary-ghost

## Difficulty

Medium

## Description

A binary ghost arranges n haunted bits in a row, numbered 1 to n. Initially, all bits are glowing (alive).
The ghost performs n hauntings. For the i‑th haunting (where i goes from 1 to n), every bit whose number j is a multiple of i flips its state. 
A glowing bit becomes dark, and a dark bit becomes glowing. After all n hauntings are cast, the ghost observes the final state of the bits. The ghost needs exactly k bits to be glowing in the end. Find the smallest possible number of bits n the ghost should start with to achieve exactly k glowing bits.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [G]. Haunting 1 flips 1: [D]. Final: 0 glowing.
If n=2, initial: [G, G]. Haunting 1 flips 1, 2: [D, D]. Haunting 2 flips 2: [D, G]. Final: 1 glowing (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [G,G,G,G,G].
Haunting 1 flips 1,2,3,4,5 -> [D,D,D,D,D].
Haunting 2 flips 2,4 -> [D,G,D,G,D].
Haunting 3 flips 3 -> [D,G,G,G,D].
Haunting 4 flips 4 -> [D,G,G,D,D].
Haunting 5 flips 5 -> [D,G,G,D,G].
Final state: 3 bits (2, 3, 5) are glowing (k=3). We can show n=4 results in only 2 glowing bits ([D,G,G,D]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of crystals required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory