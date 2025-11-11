## Title

Memory Fracture

## Slug

memory-fracture

## Difficulty

Medium

## Description

A researcher studies a sequence of n memory fragments, numbered 1 to n. Initially, all fragments are intact.  
The researcher performs n operations. For the i‑th operation (where i goes from 1 to n), every fragment whose number j is a multiple of i has its state flipped.  
An intact fragment becomes corrupted, and a corrupted fragment becomes intact. After all n operations are completed, the researcher observes the final state of the fragments. The researcher needs exactly k intact fragments in the end. Find the smallest possible number of fragments n the researcher should start with to achieve exactly k intact fragments.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [I]. Operation 1 flips 1: [C]. Final: 0 intact.  
If n=2, initial: [I, I]. Operation 1 flips 1, 2: [C, C]. Operation 2 flips 2: [C, I]. Final: 1 intact (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [I,I,I,I,I].  
Operation 1 flips 1,2,3,4,5 → [C,C,C,C,C].  
Operation 2 flips 2,4 → [C,I,C,I,C].  
Operation 3 flips 3 → [C,I,I,I,C].  
Operation 4 flips 4 → [C,I,I,C,C].  
Operation 5 flips 5 → [C,I,I,C,I].  
Final state: 3 fragments (2, 3, 5) are intact (k=3). We can show n=4 results in only 2 intact fragments ([C,I,I,C]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of fragments required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory