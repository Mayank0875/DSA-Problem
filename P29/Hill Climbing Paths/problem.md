## Title

Hill Climbing Paths

## Slug

hill-climbing-paths

## Difficulty

Easy

## Description

A hiker is climbing a series of hills. The path is made of $n$ 'up' steps and $n$ 'down' steps. A 'safe path' is one that starts at base camp, never goes *below* base camp, and finally returns to base camp. How many different safe paths can be formed with $n$ 'up' steps and $n$ 'down' steps?
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