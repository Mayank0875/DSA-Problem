## Title

Bitstream Echo

## Slug

bitstream-echo

## Difficulty

Medium

## Description

A digital engineer works with a line of n bits, indexed from 1 to n. Initially, every bit is set to 1 (ON). The engineer applies n echo operations. During the i‑th operation (for i from 1 to n), each bit whose index j is a multiple of i toggles its state: an ON bit becomes OFF, and an OFF bit becomes ON. After completing all n operations, the engineer checks the final configuration of the bits. He requires exactly k bits to be ON at the end. Determine the smallest possible length n the engineer should start with to achieve exactly k ON bits.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [1]. Operation 1 toggles 1: [0]. Final: 0 bits ON.  
If n=2, initial: [1, 1]. Operation 1 toggles 1,2: [0, 0]. Operation 2 toggles 2: [0, 1]. Final: 1 bit ON (k=1).  
Smallest n is 2.

### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [1,1,1,1,1].  
Operation 1 toggles 1,2,3,4,5 → [0,0,0,0,0].  
Operation 2 toggles 2,4 → [0,1,0,1,0].  
Operation 3 toggles 3 → [0,1,1,1,0].  
Operation 4 toggles 4 → [0,1,1,0,0].  
Operation 5 toggles 5 → [0,1,1,0,1].  
Final state: 3 bits (positions 2, 3, 5) are ON (k=3). We can show n=4 results in only 2 bits ON ([0,1,1,0]), so 5 is the minimum.

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