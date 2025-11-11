## Title

Fractal Current

## Slug

fractal-current

## Difficulty

Medium

## Description

A researcher arranges n points along a fractal conductor, numbered 1 to n. Initially, all points have current flowing.
The researcher performs n adjustments. For the i‑th adjustment (where i goes from 1 to n), every point whose number j is a multiple of i toggles its state.  
A point with current becomes without current, and a point without current becomes with current. After all n adjustments are applied, the researcher observes the final state of the points. The researcher needs exactly k points to have current in the end. Find the smallest possible number of points n the researcher should start with to achieve exactly k points with current.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [C]. Adjustment 1 toggles 1: [N]. Final: 0 points with current.  
If n=2, initial: [C, C]. Adjustment 1 toggles 1, 2: [N, N]. Adjustment 2 toggles 2: [N, C]. Final: 1 point with current (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [C,C,C,C,C].  
Adjustment 1 toggles 1,2,3,4,5 → [N,N,N,N,N].  
Adjustment 2 toggles 2,4 → [N,C,N,C,N].  
Adjustment 3 toggles 3 → [N,C,C,C,N].  
Adjustment 4 toggles 4 → [N,C,C,N,N].  
Adjustment 5 toggles 5 → [N,C,C,N,C].  
Final state: 3 points (2, 3, 5) have current (k=3). We can show n=4 results in only 2 points with current ([N,C,C,N]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of points required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory