## Title

Balanced Parentheses Count

## Slug

balanced-parentheses-count

## Difficulty

Easy

## Description

You are building a linter for a new programming language. A key feature is checking if parentheses are balanced. A sequence of parentheses is 'well-formed' if every opening parenthesis has a corresponding closing parenthesis, and they are properly nested. For example, `(())` is well-formed, but `)(` is not. Given an integer $n$, your task is to determine how many different well-formed combinations of parentheses can be created using exactly $n$ opening parentheses and $n$ closing parentheses. You just need to return the total count.
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