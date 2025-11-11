## Title

Synthetic Sequence

## Slug

synthetic-sequence

## Difficulty

Medium

## Description

A scientist synthesizes a sequence of *n* synthetic elements in a row, numbered 1 to *n*. Initially, all elements are active.  
The scientist performs *n* operations. For the *i*-th operation (where *i* goes from 1 to *n*), every element whose number *j* is a multiple of *i* toggles its state.  
An active element becomes inactive, and an inactive element becomes active. After all *n* operations are performed, the scientist observes the final state of the sequence. The scientist needs exactly *k* elements to be active in the end. Find the smallest possible number of elements *n* the scientist should start with to achieve exactly *k* active elements.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If *n*=1, initial: [A]. Operation 1 toggles 1: [I]. Final: 0 active.  
If *n*=2, initial: [A, A]. Operation 1 toggles 1, 2: [I, I]. Operation 2 toggles 2: [I, A]. Final: 1 active (*k*=1).  
Smallest *n* is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If *n*=5, initial: [A,A,A,A,A].  
Operation 1 toggles 1,2,3,4,5 → [I,I,I,I,I].  
Operation 2 toggles 2,4 → [I,A,I,A,I].  
Operation 3 toggles 3 → [I,A,A,A,I].  
Operation 4 toggles 4 → [I,A,A,I,I].  
Operation 5 toggles 5 → [I,A,A,I,A].  
Final state: 3 elements (2, 3, 5) are active (*k*=3). We can show *n*=4 results in only 2 active elements ([I,A,A,I]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer *k*.

## Output Format  

- Return one integer: the minimum number of elements required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory