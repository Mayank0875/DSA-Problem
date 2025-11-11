## Title

Phantom Recursion

## Slug

phantom-recursion

## Difficulty

Medium

## Description

A phantom traverses a line of n enchanted mirrors, numbered 1 to n. Initially, all mirrors are reflecting light.  
The phantom performs n recursive steps. For the i‑th step (where i goes from 1 to n), every mirror whose number j is a multiple of i flips its state: a reflecting mirror becomes non‑reflecting, and a non‑reflecting mirror becomes reflecting.  
After all n steps are completed, the phantom observes the final configuration of the mirrors. The phantom needs exactly k mirrors to be reflecting in the end. Find the smallest possible number of mirrors n the phantom should start with to achieve exactly k reflecting mirrors.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [R]. Step 1 flips 1: [N]. Final: 0 reflecting.  
If n=2, initial: [R, R]. Step 1 flips 1, 2: [N, N]. Step 2 flips 2: [N, R]. Final: 1 reflecting (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [R,R,R,R,R].  
Step 1 flips 1,2,3,4,5 → [N,N,N,N,N].  
Step 2 flips 2,4 → [N,R,N,R,N].  
Step 3 flips 3 → [N,R,R,R,N].  
Step 4 flips 4 → [N,R,R,N,N].  
Step 5 flips 5 → [N,R,R,N,R].  
Final state: 3 mirrors (2, 3, 5) are reflecting (k=3). We can show n=4 results in only 2 reflecting mirrors ([N,R,R,N]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of mirrors required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory