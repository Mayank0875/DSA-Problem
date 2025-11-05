## Title

Well-Formed Brackets

## Slug

well-formed-brackets

## Difficulty

Easy

## Description

You are given $n$ pairs of square brackets `[]`. A sequence of these brackets is 'well-formed' if every opening bracket `[` has a corresponding closing bracket `]`, and they are properly nested. For example, `[[]]` is well-formed, but `][` is not. Your task is to determine how many different well-formed combinations can be created using exactly $n$ opening and $n$ closing brackets.
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