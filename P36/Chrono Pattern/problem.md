## Title

Chrono Pattern

## Slug

chrono-pattern

## Difficulty

Medium

## Description

A timekeeper arranges n temporal stones in a line, numbered 1 to n. Initially, all stones are in the active state.  
The timekeeper performs n chronomantic cycles. For the i‑th cycle (where i goes from 1 to n), every stone whose number j is a multiple of i toggles its state.  
An active stone becomes dormant, and a dormant stone becomes active. After all n cycles are completed, the timekeeper observes the final configuration of the stones. The timekeeper needs exactly k stones to be active in the end. Find the smallest possible number of stones n the timekeeper should start with to achieve exactly k active stones.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [A]. Cycle 1 toggles 1: [D]. Final: 0 active.  
If n=2, initial: [A, A]. Cycle 1 toggles 1, 2: [D, D]. Cycle 2 toggles 2: [D, A]. Final: 1 active (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [A,A,A,A,A].  
Cycle 1 toggles 1,2,3,4,5 -> [D,D,D,D,D].  
Cycle 2 toggles 2,4 -> [D,A,D,A,D].  
Cycle 3 toggles 3 -> [D,A,A,A,D].  
Cycle 4 toggles 4 -> [D,A,A,D,D].  
Cycle 5 toggles 5 -> [D,A,A,D,A].  
Final state: 3 stones (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active stones ([D,A,A,D]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of stones required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory