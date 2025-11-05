## Title

Valid Sub-Array Slices

## Slug

valid-sub-array-slices

## Difficulty

Easy

## Description

You are working on an algorithm that involves $n$ 'slice start' operations and $n$ 'slice end' operations on an array. A sequence of these operations is 'valid' if every 'start' is eventually followed by an 'end', and you never 'end' a slice that hasn't 'started'. Your task is to find the total number of different valid operation sequences.
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