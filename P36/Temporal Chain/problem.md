## Title

Temporal Chain

## Slug

temporal-chain

## Difficulty

Medium

## Description

A time researcher arranges n temporal nodes in a line, numbered 1 to n. Initially, all nodes are active.
The researcher performs n temporal adjustments. For the i‑th adjustment (where i goes from 1 to n), every node whose number j is a multiple of i toggles its state.
An active node becomes inactive, and an inactive node becomes active. After all n adjustments are applied, the researcher observes the final state of the nodes. The researcher needs exactly k nodes to be active in the end. Find the smallest possible number of nodes n the researcher should start with to achieve exactly k active nodes.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [A]. Adjustment 1 toggles 1: [I]. Final: 0 active.
If n=2, initial: [A, A]. Adjustment 1 toggles 1, 2: [I, I]. Adjustment 2 toggles 2: [I, A]. Final: 1 active (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [A,A,A,A,A].
Adjustment 1 toggles 1,2,3,4,5 -> [I,I,I,I,I].
Adjustment 2 toggles 2,4 -> [I,A,I,A,I].
Adjustment 3 toggles 3 -> [I,A,A,A,I].
Adjustment 4 toggles 4 -> [I,A,A,I,I].
Adjustment 5 toggles 5 -> [I,A,A,I,A].
Final state: 3 nodes (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active nodes ([I,A,A,I]), so 5 is the minimum.
  

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