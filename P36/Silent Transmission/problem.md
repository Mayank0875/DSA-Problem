## Title

Silent Transmission

## Slug

silent-transmission

## Difficulty

Medium

## Description

A covert operation uses **n** communication nodes arranged in a line, numbered 1 to n. Initially, all nodes are silent.  
The operator performs **n** transmission cycles. For the *i*-th cycle (where *i* goes from 1 to n), every node whose number *j* is a multiple of *i* toggles its state: a silent node becomes active, and an active node becomes silent.  

After all **n** cycles are completed, the operator needs exactly **k** nodes to be active. Find the smallest possible number of nodes **n** the operator should start with to achieve exactly **k** active nodes.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [S]. Cycle 1 toggles 1: [A]. Final: 0 active.  
If n=2, initial: [S, S]. Cycle 1 toggles 1, 2: [A, A]. Cycle 2 toggles 2: [A, S]. Final: 1 active (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [S,S,S,S,S].  
Cycle 1 toggles 1,2,3,4,5 → [A,A,A,A,A].  
Cycle 2 toggles 2,4 → [A,S,A,S,A].  
Cycle 3 toggles 3 → [A,S,A,S,A].  
Cycle 4 toggles 4 → [A,S,A,S,A].  
Cycle 5 toggles 5 → [A,S,A,S,A].  
Final state: 3 nodes (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active nodes ([A,S,A,S]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of nodes required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory