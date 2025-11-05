## Title

Magic Spell Chants

## Slug

magic-spell-chants

## Difficulty

Easy

## Description

A powerful magic spell requires a sequence of $n$ 'In' chants and $n$ 'Out' chants. The spell is 'stable' only if the chants are correctly nested, meaning every 'In' has a matching 'Out' and you never chant 'Out' unless a corresponding 'In' has already been chanted. Your task is to calculate the total number of distinct, stable chant sequences.
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