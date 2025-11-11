## Title

Lost Signal Recovery

## Slug

lost-signal

## Difficulty

Medium

## Description

A radio operator monitors **n** signal towers arranged in a line, numbered 1 to n. Initially, all towers are transmitting a clear signal.  
The operator performs **n** interference cycles. For the *i*-th cycle (where *i* goes from 1 to n), every tower whose number *j* is a multiple of *i* flips its state: a transmitting tower becomes silent, and a silent tower becomes transmitting.  
After all n cycles are completed, the operator observes the final state of the towers. He needs exactly **k** towers to be transmitting in the end. Find the smallest possible number of towers **n** the operator should start with to achieve exactly **k** transmitting towers.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [T]. Cycle 1 flips 1: [S]. Final: 0 transmitting.  
If n=2, initial: [T, T]. Cycle 1 flips 1, 2: [S, S]. Cycle 2 flips 2: [S, T]. Final: 1 transmitting (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [T,T,T,T,T].  
Cycle 1 flips 1,2,3,4,5 → [S,S,S,S,S].  
Cycle 2 flips 2,4 → [S,T,S,T,S].  
Cycle 3 flips 3 → [S,T,T,T,S].  
Cycle 4 flips 4 → [S,T,T,S,S].  
Cycle 5 flips 5 → [S,T,T,S,T].  
Final state: 3 towers (2, 3, 5) are transmitting (k=3). We can show n=4 results in only 2 transmitting towers ([S,T,T,S]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of towers required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory