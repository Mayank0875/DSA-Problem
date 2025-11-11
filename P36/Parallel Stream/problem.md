## Title

Parallel Stream

## Slug

parallel-stream

## Difficulty

Medium

## Description

A system processes **n** parallel data streams, numbered 1 to n. Initially, all streams are active (ON).  
The system performs **n** synchronization steps. For the *i*-th step (where *i* goes from 1 to n), every stream whose number *j* is a multiple of *i* toggles its state: an active stream becomes inactive (OFF), and an inactive stream becomes active (ON).  
After all **n** steps are completed, the system requires exactly **k** streams to be active. Find the smallest possible number of streams **n** the system should start with to achieve exactly **k** active streams.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [ON]. Step 1 toggles 1: [OFF]. Final: 0 active.  
If n=2, initial: [ON, ON]. Step 1 toggles 1, 2: [OFF, OFF]. Step 2 toggles 2: [OFF, ON]. Final: 1 active (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [ON,ON,ON,ON,ON].  
Step 1 toggles 1,2,3,4,5 → [OFF,OFF,OFF,OFF,OFF].  
Step 2 toggles 2,4 → [OFF,ON,OFF,ON,OFF].  
Step 3 toggles 3 → [OFF,ON,ON,ON,OFF].  
Step 4 toggles 4 → [OFF,ON,ON,OFF,OFF].  
Step 5 toggles 5 → [OFF,ON,ON,OFF,ON].  
Final state: 3 streams (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active streams ([OFF,ON,ON,OFF]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of streams required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory