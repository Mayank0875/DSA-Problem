## Title

Encrypted Valley

## Slug

encrypted-valley

## Difficulty

Medium

## Description

A cryptographer arranges n data nodes in a line, numbered 1 to n. Initially, all nodes are unencrypted.  
The cryptographer performs n encryption rounds. For the i‑th round (where i goes from 1 to n), every node whose number j is a multiple of i toggles its state.  
An unencrypted node becomes encrypted, and an encrypted node becomes unencrypted. After all n rounds are completed, the cryptographer observes the final state of the nodes. He needs exactly k nodes to be encrypted in the end. Find the smallest possible number of nodes n the cryptographer should start with to achieve exactly k encrypted nodes.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [U]. Round 1 toggles 1: [E]. Final: 0 encrypted.  
If n=2, initial: [U, U]. Round 1 toggles 1, 2: [E, E]. Round 2 toggles 2: [E, U]. Final: 1 encrypted (k=1).  
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [U,U,U,U,U].  
Round 1 toggles 1,2,3,4,5 → [E,E,E,E,E].  
Round 2 toggles 2,4 → [E,U,E,U,E].  
Round 3 toggles 3 → [E,U,E,U,E].  
Round 4 toggles 4 → [E,U,E,U,E].  
Round 5 toggles 5 → [E,U,E,U,E].  
Final state: 3 nodes (2, 3, 5) are encrypted (k=3). We can show n=4 results in only 2 encrypted nodes ([E,U,U,E]), so 5 is the minimum.
  

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