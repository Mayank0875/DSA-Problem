## Title

Recursive Tide

## Slug

recursive-tide

## Difficulty

Medium

## Description

A coastal guardian monitors n tide markers placed along the shoreline, numbered 1 to n. Initially, all markers are in a high tide state.
The guardian performs n tidal cycles. For the i‑th cycle (where i goes from 1 to n), every marker whose number j is a multiple of i switches its state. 
A high tide marker becomes low tide, and a low tide marker becomes high tide. After all n cycles are completed, the guardian observes the final state of the markers. The guardian needs exactly k markers to be in a high tide state in the end. Find the smallest possible number of markers n the guardian should start with to achieve exactly k high tide markers.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [H]. Cycle 1 flips 1: [L]. Final: 0 high tide.
If n=2, initial: [H, H]. Cycle 1 flips 1, 2: [L, L]. Cycle 2 flips 2: [L, H]. Final: 1 high tide (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [H,H,H,H,H].
Cycle 1 flips 1,2,3,4,5 -> [L,L,L,L,L].
Cycle 2 flips 2,4 -> [L,H,L,H,L].
Cycle 3 flips 3 -> [L,H,H,H,L].
 Cycle 4 flips 4 -> [L,H,H,L,L].
 Cycle 5 flips 5 -> [L,H,H,L,H].
Final state: 3 markers (2, 3, 5) are high tide (k=3). We can show n=4 results in only 2 high tide markers ([L,H,H,L]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of markers required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory