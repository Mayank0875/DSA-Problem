## Title

Wizard's Crystal Grid

## Slug

wizards-crystal-grid

## Difficulty

Medium

## Description

A wizard arranges n magical crystals in a row, numbered 1 to n. Initially, all crystals are glowing.
The wizard performs n spells. For the i-th spell (where i goes from 1 to n), every crystal whose number j is a multiple of i flips its state. 
A glowing crystal becomes dark, and a dark crystal becomes glowing. After all n spells are cast, the wizard observes the final state of the crystals. The wizard needs exactly k crystals to be glowing in the end. Find the smallest possible number of crystals n the wizard should start with to achieve exactly k glowing crystals.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [G]. Spell 1 flips 1: [D]. Final: 0 glowing.
If n=2, initial: [G, G]. Spell 1 flips 1, 2: [D, D]. Spell 2 flips 2: [D, G]. Final: 1 glowing (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [G,G,G,G,G].
Spell 1 flips 1,2,3,4,5 -> [D,D,D,D,D].
Spell 2 flips 2,4 -> [D,G,D,G,D].
Spell 3 flips 3 -> [D,G,G,G,D].
Spell 4 flips 4 -> [D,G,G,D,D].
Spell 5 flips 5 -> [D,G,G,D,G].
Final state: 3 crystals (2, 3, 5) are glowing (k=3). We can show n=4 results in only 2 glowing crystals ([D,G,G,D]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of crystals required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory