## Title

Valid XML Structures

## Slug

valid-xml-structures

## Difficulty

Easy

## Description

You are given $n$ pairs of angle brackets `<>`. A 'valid structure' is one where every opening bracket `<` has a corresponding closing bracket `>`, and they are properly nested (e.g., `<><>`). Your task is to determine how many different valid structures can be created using exactly $n$ opening and $n$ closing brackets.
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