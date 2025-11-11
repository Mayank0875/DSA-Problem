## Title

Temporal Code Sequence

## Slug

temporal-code

## Difficulty

Medium

## Description

A chronomancer arranges n temporal codes in a line, numbered 1 to n. Initially, all codes are active.  
The chronomancer performs n temporal shifts. For the i-th shift (where i goes from 1 to n), every code whose number j is a multiple of i toggles its state.  
An active code becomes inactive, and an inactive code becomes active. After all n shifts are applied, the chronomancer observes the final state of the codes. The chronomancer needs exactly k codes to be active in the end. Find the smallest possible number of codes n the chronomancer should start with to achieve exactly k active codes.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [A]. Shift 1 toggles 1: [I]. Final: 0 active.  
If n=2, initial: [A, A]. Shift 1 toggles 1, 2: [I, I]. Shift 2 toggles 2: [I, A]. Final: 1 active (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [A,A,A,A,A].  
Shift 1 toggles 1,2,3,4,5 -> [I,I,I,I,I].  
Shift 2 toggles 2,4 -> [I,A,I,A,I].  
Shift 3 toggles 3 -> [I,A,A,A,I].  
Shift 4 toggles 4 -> [I,A,A,I,I].  
Shift 5 toggles 5 -> [I,A,A,I,A].  
Final state: 3 codes (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active codes ([I,A,A,I]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of codes required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory