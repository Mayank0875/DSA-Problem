## Title

Echoes of Infinity

## Slug

echoes-of-infinity

## Difficulty

Medium

## Description

An ancient astronomer aligns **n** resonant spheres in a straight line, numbered from 1 to n. Initially, every sphere emits a bright pulse.  
The astronomer then performs **n** reverberations. For the *i*‑th reverberation (where *i* goes from 1 to n), every sphere whose number *j* is a multiple of *i* flips its pulse state: a bright pulse becomes silent, and a silent sphere begins to pulse.  
After all n reverberations have echoed, the astronomer observes the final pattern of pulses. He requires exactly **k** spheres to be pulsing at the end. Determine the smallest possible number of spheres **n** the astronomer should start with to achieve exactly **k** pulsing spheres.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [P]. Reverberation 1 flips 1: [S]. Final: 0 pulsing.  
If n=2, initial: [P, P]. Reverberation 1 flips 1, 2: [S, S]. Reverberation 2 flips 2: [S, P]. Final: 1 pulsing (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [P,P,P,P,P].  
Reverberation 1 flips 1,2,3,4,5 → [S,S,S,S,S].  
Reverberation 2 flips 2,4 → [S,P,S,P,S].  
Reverberation 3 flips 3 → [S,P,P,P,S].  
Reverberation 4 flips 4 → [S,P,P,S,S].  
Reverberation 5 flips 5 → [S,P,P,S,P].  
Final state: 3 spheres (2, 3, 5) are pulsing (k=3). We can show n=4 results in only 2 pulsing spheres ([S,P,P,S]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of spheres required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory