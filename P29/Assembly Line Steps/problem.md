## Title

Assembly Line Steps

## Slug

assembly-line-steps

## Difficulty

Easy

## Description

An assembly line has $n$ 'start process' steps and $n$ 'end process' steps. A 'valid' assembly sequence must be 'nested' correctly: every 'start' must have a matching 'end', and no process can 'end' before it has 'started'. Your job is to count the total number of unique, valid assembly sequences.
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