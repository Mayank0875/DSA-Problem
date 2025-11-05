## Title

Valid Stack Operations

## Slug

valid-stack-operations

## Difficulty

Easy

## Description

You are analyzing a sequence of stack operations. You have $n$ 'push' operations and $n$ 'pop' operations. A sequence is 'valid' if you never try to pop from an empty stack. Your task is to find the total number of different valid sequences that can be formed using exactly $n$ pushes and $n$ pops. This count represents all possible valid execution paths.
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