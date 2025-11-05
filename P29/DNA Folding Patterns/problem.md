## Title

DNA Folding Patterns

## Slug

dna-folding-patterns

## Difficulty

Easy

## Description

A strand of DNA has $n$ 'A' bases and $n$ 'T' bases. A 'folding' is represented by a sequence of these bases. A 'stable' folding requires that every 'A' can be paired with a 'T' that comes after it, and the pairs are properly nested, like parentheses. For $n$ pairs, how many different stable folding sequences are possible?
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