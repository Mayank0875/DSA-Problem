## Title

Quantum Pulse Sequence

## Slug

quantum-pulse-sequence

## Difficulty

Medium

## Description

A quantum physicist arranges n quantum pulses in a line, numbered 1 to n. Initially, all pulses are active.  
The physicist performs n operations. For the i‑th operation (where i goes from 1 to n), every pulse whose number j is a multiple of i flips its state.  
An active pulse becomes inactive, and an inactive pulse becomes active. After all n operations are performed, the physicist observes the final state of the pulses. The physicist needs exactly k pulses to be active in the end. Find the smallest possible number of pulses n the physicist should start with to achieve exactly k active pulses.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [A]. Operation 1 flips 1: [I]. Final: 0 active.  
If n=2, initial: [A, A]. Operation 1 flips 1, 2: [I, I]. Operation 2 flips 2: [I, A]. Final: 1 active (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [A,A,A,A,A].  
Operation 1 flips 1,2,3,4,5 → [I,I,I,I,I].  
Operation 2 flips 2,4 → [I,A,I,A,I].  
Operation 3 flips 3 → [I,A,A,A,I].  
Operation 4 flips 4 → [I,A,A,I,I].  
Operation 5 flips 5 → [I,A,A,I,A].  
Final state: 3 pulses (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active pulses ([I,A,A,I]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of pulses required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory