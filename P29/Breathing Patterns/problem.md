## Title

Breathing Patterns

## Slug

breathing-patterns

## Difficulty

Easy

## Description

You are modeling breathing patterns. A pattern consists of $n$ 'Inhales' and $n$ 'Exhales'. A 'natural' breathing pattern is a sequence where one must 'Inhale' before they can 'Exhale', and the pattern starts and ends at a neutral state. How many different 'natural' patterns can be formed with $n$ inhales and $n$ exhales?
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