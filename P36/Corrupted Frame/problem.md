## Title

Corrupted Frame

## Slug

corrupted-frame

## Difficulty

Medium

## Description

A digital forensics analyst is examining a sequence of n video frames, numbered 1 to n. Initially, all frames are clean.  
The analyst runs n integrity checks. For the i‑th check (where i goes from 1 to n), every frame whose number j is a multiple of i gets its corruption flag toggled.  
A clean frame becomes corrupted, and a corrupted frame becomes clean. After all n checks are performed, the analyst looks at the final state of the frames. He needs exactly k frames to remain clean in the end. Find the smallest possible number of frames n the analyst should start with to achieve exactly k clean frames.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [C]. Check 1 flips 1: [X]. Final: 0 clean.  
If n=2, initial: [C, C]. Check 1 flips 1, 2: [X, X]. Check 2 flips 2: [X, C]. Final: 1 clean (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [C,C,C,C,C].  
Check 1 flips 1,2,3,4,5 → [X,X,X,X,X].  
Check 2 flips 2,4 → [X,C,X,C,X].  
Check 3 flips 3 → [X,C,C,C,X].  
Check 4 flips 4 → [X,C,C,X,X].  
Check 5 flips 5 → [X,C,C,X,C].  
Final state: 3 frames (2, 3, 5) are clean (k=3). We can show n=4 results in only 2 clean frames ([X,C,C,X]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of frames required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory