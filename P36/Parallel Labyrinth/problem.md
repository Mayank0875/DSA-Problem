## Title

Parallel Labyrinth

## Slug

parallel-labyrinth

## Difficulty

Medium

## Description

An adventurer explores a parallel labyrinth consisting of n chambers arranged in a line, numbered 1 to n. Initially, all chambers are lit.
The adventurer performs n passes through the labyrinth. For the i‑th pass (where i goes from 1 to n), every chamber whose number j is a multiple of i toggles its light state. 
A lit chamber becomes dark, and a dark chamber becomes lit. After all n passes are completed, the adventurer observes the final illumination of the chambers. The adventurer needs exactly k chambers to remain lit in the end. Find the smallest possible number of chambers n the labyrinth should contain to achieve exactly k lit chambers.

## Examples

### 1

#### Input

1

#### Output

2

#### Explanation

If n=1, initial: [L]. Pass 1 toggles 1: [D]. Final: 0 lit.
If n=2, initial: [L, L]. Pass 1 toggles 1, 2: [D, D]. Pass 2 toggles 2: [D, L]. Final: 1 lit (k=1).
Smallest n is 2.
    
### 2

#### Input

3

#### Output

5

#### Explanation
If n=5, initial: [L,L,L,L,L].
Pass 1 toggles 1,2,3,4,5 -> [D,D,D,D,D].
Pass 2 toggles 2,4 -> [D,L,D,L,D].
Pass 3 toggles 3 -> [D,L,L,L,D].
Pass 4 toggles 4 -> [D,L,L,D,D].
Pass 5 toggles 5 -> [D,L,L,D,L].
Final state: 3 chambers (2, 3, 5) are lit (k=3). We can show n=4 results in only 2 lit chambers ([D,L,L,D]), so 5 is the minimum.
  

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return one integer: the minimum number of chambers required.
  

## Constraints  

- 1 ≤ x ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory