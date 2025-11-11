## Title

Logic Paradox Grid

## Slug

logic-paradox-grid

## Difficulty

Medium

## Description

A logician writes down n statements in a row, numbered 1 to n. Initially, every statement is true.  
The logician then performs n paradoxical operations. For the i‑th operation (where i goes from 1 to n), every statement whose number j is a multiple of i flips its truth value: a true statement becomes false, and a false statement becomes true.  

After all n operations are applied, the logician observes the final truth values of the statements. He needs exactly k statements to be true in the end. Find the smallest possible number of statements n the logician should start with to achieve exactly k true statements.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [T]. Operation 1 flips 1: [F]. Final: 0 true.  
If n=2, initial: [T, T]. Operation 1 flips 1, 2: [F, F]. Operation 2 flips 2: [F, T]. Final: 1 true (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [T,T,T,T,T].  
Operation 1 flips 1,2,3,4,5 → [F,F,F,F,F].  
Operation 2 flips 2,4 → [F,T,F,T,F].  
Operation 3 flips 3 → [F,T,T,T,F].  
Operation 4 flips 4 → [F,T,T,F,F].  
Operation 5 flips 5 → [F,T,T,F,T].  
Final state: 3 statements (2, 3, 5) are true (k=3). We can show n=4 results in only 2 true statements ([F,T,T,F]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of statements required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory