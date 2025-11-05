## Title

Recursive Call Count

## Slug

recursive-call-count

## Difficulty

Easy

## Description

You are analyzing a recursive function. The function will 'call' itself $n$ times and 'return' $n$ times. A 'valid' execution path is a sequence of these calls and returns where a 'return' only happens after a 'call', and the number of 'returns' never exceeds the number of 'calls'. How many different valid execution paths are there for $n$ calls?
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