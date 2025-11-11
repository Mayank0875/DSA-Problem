## Title

The Hidden Byte

## Slug

hidden-byte

## Difficulty

Medium

## Description

A programmer has an array of n bytes, indexed from 1 to n. Initially, every byte is set to 1 (“on”).  
The programmer runs n operations. For the i‑th operation (where i runs from 1 to n), every byte whose index j is a multiple of i toggles its value: a 1 becomes 0, and a 0 becomes 1.  
After all n operations have been performed, the programmer checks the final state of the array. He needs exactly k bytes to be 1 in the end. Determine the smallest possible n the programmer should start with to achieve exactly k bytes set to 1.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [1]. Operation 1 toggles 1: [0]. Final: 0 bytes set to 1.  
If n=2, initial: [1, 1]. Operation 1 toggles 1, 2: [0, 0]. Operation 2 toggles 2: [0, 1]. Final: 1 byte set to 1 (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [1,1,1,1,1].  
Operation 1 toggles 1,2,3,4,5 → [0,0,0,0,0].  
Operation 2 toggles 2,4 → [0,1,0,1,0].  
Operation 3 toggles 3 → [0,1,1,1,0].  
Operation 4 toggles 4 → [0,1,1,0,0].  
Operation 5 toggles 5 → [0,1,1,0,1].  
Final state: 3 bytes (positions 2, 3, 5) are 1 (k=3). We can show n=4 results in only 2 bytes set to 1 ([0,1,1,0]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of bytes required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory