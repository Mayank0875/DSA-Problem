## Title

The Obsidian Key

## Slug

the-obsidian-key

## Difficulty

Medium

## Description

A master locksmith arranges n obsidian key fragments in a row, numbered 1 to n. Initially, all fragments are active.
The locksmith performs n rituals. For the i‑th ritual (where i goes from 1 to n), every fragment whose number j is a multiple of i toggles its state. 
An active fragment becomes inactive, and an inactive fragment becomes active. After all n rituals are performed, the locksmith observes the final state of the fragments. The locksmith needs exactly k fragments to be active in the end. Find the smallest possible number of fragments n the locksmith should start with to achieve exactly k active fragments.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [G]. Ritual 1 flips 1: [D]. Final: 0 active.
If n=2, initial: [G, G]. Ritual 1 flips 1, 2: [D, D]. Ritual 2 flips 2: [D, G]. Final: 1 active (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [G,G,G,G,G].
Ritual 1 flips 1,2,3,4,5 -> [D,D,D,D,D].
Ritual 2 flips 2,4 -> [D,G,D,G,D].
Ritual 3 flips 3 -> [D,G,G,G,D].
Ritual 4 flips 4 -> [D,G,G,D,D].
Ritual 5 flips 5 -> [D,G,G,D,G].
Final state: 3 fragments (2, 3, 5) are active (k=3). We can show n=4 results in only 2 active fragments ([D,G,G,D]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of fragments required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory