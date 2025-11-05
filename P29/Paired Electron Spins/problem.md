## Title

Paired Electron Spins

## Slug

paired-electron-spins

## Difficulty

Easy

## Description

In a simplified model of physics, $n$ electrons have 'spin up' and $n$ electrons have 'spin down'. They must be paired. A 'stable' configuration is a sequence of spins where every 'spin up' has a matching 'spin down', and the total spin is never negative (never more 'down' than 'up'). How many stable configurations are possible?
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