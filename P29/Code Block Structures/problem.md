## Title

Code Block Structures

## Slug

code-block-structures

## Difficulty

Easy

## Description

A new coding language uses `{` to open a code block and `}` to close one. A 'valid' program structure must have all blocks properly nested. For example, `{{}}` is valid, but `{}}{` is not. Given $n$ pairs of braces, your task is to count how many different valid program structures can be formed using exactly $n$ opening and $n$ closing braces.
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