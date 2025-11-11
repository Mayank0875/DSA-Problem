## Title

Spectral Array

## Slug

spectral-array

## Difficulty

Medium

## Description

A researcher arranges n spectral elements in a line, numbered 1 to n. Initially, all elements emit light.  
The researcher performs n operations. For the i‑th operation (where i goes from 1 to n), every element whose index j is a multiple of i toggles its emission state.  
An emitting element becomes non‑emitting, and a non‑emitting element becomes emitting. After all n operations are performed, the researcher observes the final configuration. The researcher needs exactly k elements to be emitting in the end. Find the smallest possible number of elements n the researcher should start with to achieve exactly k emitting elements.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [E]. Operation 1 toggles 1: [N]. Final: 0 emitting.  
If n=2, initial: [E, E]. Operation 1 toggles 1, 2: [N, N]. Operation 2 toggles 2: [N, E]. Final: 1 emitting (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [E,E,E,E,E].  
Operation 1 toggles 1,2,3,4,5 → [N,N,N,N,N].  
Operation 2 toggles 2,4 → [N,E,N,E,N].  
Operation 3 toggles 3 → [N,E,E,E,N].  
Operation 4 toggles 4 → [N,E,E,N,N].  
Operation 5 toggles 5 → [N,E,E,N,E].  
Final state: 3 elements (2, 3, 5) are emitting (k=3). We can show n=4 results in only 2 emitting elements ([N,E,E,N]), so 5 is the minimum.
  

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