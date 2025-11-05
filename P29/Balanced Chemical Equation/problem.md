## Title

Balanced Chemical Equation

## Slug

balanced-chemical-equation

## Difficulty

Easy

## Description

You are modeling a simple chemical reaction with $n$ 'bond' (create) events and $n$ 'break' (destroy) events. A 'stable' reaction pathway is a sequence where a bond never 'breaks' unless it has been 'created', and all 'create' events are matched. How many different stable reaction pathways are there for $n$ pairs?
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