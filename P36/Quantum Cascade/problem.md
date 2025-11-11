## Title

Quantum Cascade

## Slug

quantum-cascade

## Difficulty

Medium

## Description

A physicist arranges **n** quantum particles in a line, numbered 1 to n. Initially, all particles are in the excited state.  
The physicist triggers **n** cascade steps. For the *i*-th step (where *i* goes from 1 to n), every particle whose number *j* is a multiple of *i* toggles its state.  
An excited particle becomes grounded, and a grounded particle becomes excited. After all n steps are performed, the physicist observes the final state of the particles. The physicist needs exactly **k** particles to be excited in the end. Find the smallest possible number of particles **n** the physicist should start with to achieve exactly **k** excited particles.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [G]. Spell 1 flips 1: [D]. Final: 0 glowing.  
If n=2, initial: [G, G]. Spell 1 flips 1, 2: [D, D]. Spell 2 flips 2: [D, G]. Final: 1 glowing (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [G,G,G,G,G].  
Spell 1 flips 1,2,3,4,5 -> [D,D,D,D,D].  
Spell 2 flips 2,4 -> [D,G,D,G,D].  
Spell 3 flips 3 -> [D,G,G,G,D].  
Spell 4 flips 4 -> [D,G,G,D,D].  
Spell 5 flips 5 -> [D,G,G,D,G].  
Final state: 3 crystals (2, 3, 5) are glowing (k=3). We can show n=4 results in only 2 glowing crystals ([D,G,G,D]), so 5 is the minimum.
  

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