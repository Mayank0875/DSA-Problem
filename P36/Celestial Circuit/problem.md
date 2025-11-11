## Title

Celestial Circuit

## Slug

celestial-circuit

## Difficulty

Medium

## Description

An astronomer sets up a line of n celestial beacons, numbered 1 to n. Initially, all beacons are shining.
The astronomer activates n cycles. For the i‑th cycle (where i goes from 1 to n), every beacon whose number j is a multiple of i toggles its state. 
A shining beacon becomes dim, and a dim beacon becomes shining. After all n cycles are completed, the astronomer observes the final state of the beacons. The astronomer needs exactly k beacons to be shining in the end. Find the smallest possible number of beacons n the astronomer should start with to achieve exactly k shining beacons.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [S]. Cycle 1 toggles 1: [D]. Final: 0 shining.
If n=2, initial: [S, S]. Cycle 1 toggles 1, 2: [D, D]. Cycle 2 toggles 2: [D, S]. Final: 1 shining (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [S,S,S,S,S].
Cycle 1 toggles 1,2,3,4,5 -> [D,D,D,D,D].
Cycle 2 toggles 2,4 -> [D,S,D,S,D].
Cycle 3 toggles 3 -> [D,S,S,S,D].
Cycle 4 toggles 4 -> [D,S,S,D,D].
Cycle 5 toggles 5 -> [D,S,S,D,S].
Final state: 3 beacons (2, 3, 5) are shining (k=3). We can show n=4 results in only 2 shining beacons ([D,S,S,D]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of beacons required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory