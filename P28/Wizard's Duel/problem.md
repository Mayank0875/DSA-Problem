## Title

Wizard's Duel

## Slug

wizards-duel

## Difficulty

Medium

## Description

In a formal wizard's duel, `n` wizards stand on an `n x n` arena. A wizard is considered "in danger" if another wizard is in their row, column, or diagonal. How many ways can `n` wizards be placed on the `n x n` arena so that no wizard is in danger from another?
## Examples

### 1

#### Input

1

#### Output

1

#### Explanation

On a 1x1 board, there is only one square, and placing one queen there is a valid solution.
    
### 2

#### Input

4

#### Output

2

#### Explanation
There are two distinct ways to place 4 queens on a 4x4 board safely.

## Input Format  

- The input consists of a single line containing one integer, `n`.

## Output Format  

- Return single integer representing the total number of distinct solutions.
  

## Constraints  

- 1 ≤ n ≤ 8

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion