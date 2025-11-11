## Title

The Vanishing Loop

## Slug

the-vanishing-loop

## Difficulty

Medium

## Description

A programmer writes a loop that processes n binary cells arranged in a row, numbered 1 to n. Initially, every cell holds the value 1 (“on”).  
The loop runs n passes. On the i‑th pass (where i goes from 1 to n), it toggles every cell whose index j is a multiple of i: a cell with value 1 becomes 0, and a cell with value 0 becomes 1. After completing all n passes, the programmer checks the final configuration. He needs exactly k cells to be “on” at the end. Determine the smallest possible number of cells n the programmer should start with to achieve exactly k “on” cells.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [1]. Pass 1 toggles 1: [0]. Final: 0 on.
If n=2, initial: [1, 1]. Pass 1 toggles 1, 2: [0, 0]. Pass 2 toggles 2: [0, 1]. Final: 1 on (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [1,1,1,1,1].
Pass 1 toggles 1,2,3,4,5 -> [0,0,0,0,0].
Pass 2 toggles 2,4 -> [0,1,0,1,0].
Pass 3 toggles 3 -> [0,1,1,1,0].
Pass 4 toggles 4 -> [0,1,1,0,0].
Pass 5 toggles 5 -> [0,1,1,0,1].
Final state: 3 cells (2, 3, 5) are on (k=3). We can show n=4 results in only 2 on cells ([0,1,1,0]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of cells required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory