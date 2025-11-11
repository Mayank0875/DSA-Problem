## Title

Infinite Loopstorm

## Slug

infinite-loopstorm

## Difficulty

Medium

## Description

A programmer is caught in an infinite loopstorm and has **n** servers arranged in a line, numbered 1 to n. Initially, all servers are active.  
The programmer executes **n** cycles. For the *i*-th cycle (where *i* goes from 1 to n), every server whose number *j* is a multiple of *i* toggles its state: an active server becomes inactive, and an inactive server becomes active.  

After all **n** cycles are completed, the programmer observes the final state of the servers. He needs exactly **k** servers to be active in the end. Find the smallest possible number of servers **n** the programmer should start with to achieve exactly **k** active servers.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [A]. Cycle 1 toggles 1: [I]. Final: 0 active.  
If n=2, initial: [A, A]. Cycle 1 toggles 1, 2: [I, I]. Cycle 2 toggles 2: [I, A]. Final: 1 active (k=1).  
Smallest n is 2.

### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [A,A,A,A,A].  
Cycle 1 toggles 1,2,3,4,5 → [I,I,I,I,I].  
Cycle 2 toggles 2,4 → [I,A,I,A,I].  
Cycle 3 toggles 3 → [I,A,A,A,I].  
Cycle 4 toggles 4 → [I,A,A,I,I].  
Cycle 5 toggles 5 → [I,A,A,I,A].  
Final state: 3 servers (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active servers ([I,A,A,I]), so 5 is the minimum.

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of servers required.

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory