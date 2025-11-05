## Title

Lock Mechanism Combinations

## Slug

lock-mechanism-combinations

## Difficulty

Easy

## Description

A complex lock has a mechanism involving $n$ 'engaging' tumblers and $n$ 'releasing' tumblers. A 'valid' opening sequence requires a series of $2n$ total actions. The lock only opens if every 'engage' action is matched by a 'release' action, and the mechanism never 'releases' unless it has first been 'engaged'. How many valid opening sequences exist?
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