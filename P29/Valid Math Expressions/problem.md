## Title

Valid Math Expressions

## Slug

valid-math-expressions

## Difficulty

Easy

## Description

You are a math professor teaching order of operations. You want to show your students how many ways $n$ pairs of parentheses can be placed to be 'mathematically valid'. A sequence is valid if every `(` has a matching `)` and they are nested correctly. For $n$ pairs, how many valid, distinct sequences are there?
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