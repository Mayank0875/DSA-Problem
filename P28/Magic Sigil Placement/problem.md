## Title

Magic Sigil Placement

## Slug

magic-sigil-placement

## Difficulty

Medium

## Description

A wizard is inscribing `n` powerful sigils on an `n x n` magic tablet. If any two sigils align in the same row, column, or diagonal, their magic interferes and the enchantment fails. Your task is to count the total number of safe arrangements for `n` sigils on the `n x n` tablet.
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