## Title

Binary Bloom

## Slug

binary-bloom

## Difficulty

Medium

## Description

A gardener plants n binary flowers in a row, numbered 1 to n. Initially, all flowers are in bloom.
The gardener performs n watering cycles. For the i-th cycle (where i goes from 1 to n), every flower whose number j is a multiple of i flips its state. 
A blooming flower wilts, and a wilted flower blooms. After all n cycles are completed, the gardener observes the final state of the flowers. The gardener needs exactly k flowers to be blooming in the end. Find the smallest possible number of flowers n the gardener should start with to achieve exactly k blooming flowers.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [B]. Cycle 1 flips 1: [W]. Final: 0 blooming.
If n=2, initial: [B, B]. Cycle 1 flips 1, 2: [W, W]. Cycle 2 flips 2: [W, B]. Final: 1 blooming (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [B,B,B,B,B].
Cycle 1 flips 1,2,3,4,5 -> [W,W,W,W,W].
Cycle 2 flips 2,4 -> [W,B,W,B,W].
Cycle 3 flips 3 -> [W,B,B,B,W].
Cycle 4 flips 4 -> [W,B,B,W,W].
Cycle 5 flips 5 -> [W,B,B,W,B].
Final state: 3 flowers (2, 3, 5) are blooming (k=3). We can show n=4 results in only 2 blooming flowers ([W,B,B,W]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of flowers required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory