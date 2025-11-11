## Title

The Phantom Cipher

## Slug

phantom-cipher

## Difficulty

Medium

## Description

A cryptographer prepares a sequence of n bits, numbered 1 to n, all initially set to 1 (“on”).  
The cryptographer then applies n operations. For the i‑th operation (where i runs from 1 to n), every bit whose position j is a multiple of i has its value flipped: a 1 becomes 0, and a 0 becomes 1.  
After performing all n operations, the cryptographer observes the final configuration of the bits. He requires exactly k bits to be 1 in the final state. Determine the smallest possible length n of the initial sequence that yields exactly k bits set to 1 after all operations.

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