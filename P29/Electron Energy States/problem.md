## Title

Electron Energy States

## Slug

electron-energy-states

## Difficulty

Easy

## Description

In a quantum model, an electron can jump to a higher energy state (an 'excitation') or drop to a lower state (a 'decay'). You are tracking $n$ excitations and $n$ decays. A 'stable' history requires that the electron never 'decays' unless it has been 'excited' first. How many different stable histories are possible with $n$ excitations and $n$ decays?
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