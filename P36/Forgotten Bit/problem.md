## Title

Forgotten Bit

## Slug

forgotten-bit

## Difficulty

Medium

## Description

A programmer stores n bits in a linear memory array, indexed from 1 to n. Initially, all bits are set to 1 (on).  
The programmer executes n passes. For the i‑th pass (where i goes from 1 to n), every bit whose index j is a multiple of i toggles its value: a 1 becomes 0, and a 0 becomes 1. After all n passes are completed, the programmer checks the final configuration of the bits. He needs exactly k bits to be on (value 1) in the end. Find the smallest possible number of bits n the programmer should start with to achieve exactly k bits on.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [1]. Pass 1 toggles 1: [0]. Final: 0 bits on.  
If n=2, initial: [1, 1]. Pass 1 toggles 1, 2: [0, 0]. Pass 2 toggles 2: [0, 1]. Final: 1 bit on (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [1,1,1,1,1].  
Pass 1 toggles 1,2,3,4,5 → [0,0,0,0,0].  
Pass 2 toggles 2,4 → [0,1,0,1,0].  
Pass 3 toggles 3 → [0,1,1,1,0].  
Pass 4 toggles 4 → [0,1,1,0,0].  
Pass 5 toggles 5 → [0,1,1,0,1].  
Final state: 3 bits (positions 2, 3, 5) are on (k=3). We can show n=4 results in only 2 bits on ([0,1,1,0]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of bits required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory