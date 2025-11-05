## Title

Robot Grid Paths

## Slug

robot-grid-paths

## Difficulty

Easy

## Description

A robot starts at (0, 0) and must reach (n, n) on a 2D grid. The robot can only move 'Up' or 'Right'. However, the robot must never move *above* the diagonal line $y = x$. This means the number of 'Up' moves must never exceed the number of 'Right' moves at any point. How many different valid paths can the robot take?
## Examples

### 1

#### Input

3

#### Output

5

#### Explanation

The 5 unique well-formed combinations are:
((()))
(()())
(())()
()(())
()()()

### 2

#### Input

1

#### Output

1

#### Explanation
The only combination is ().

## Input Format  

- The input consists of a single line containing one integer, `n`.

## Output Format  

- Return single integer representing total number of well-formed parenthesis combinations.
  

## Constraints  

- 1 ≤ n ≤ 8

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion