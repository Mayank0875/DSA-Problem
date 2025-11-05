## Title

Nested Box Combinations

## Slug

nested-box-combinations

## Difficulty

Easy

## Description

You have $n$ large boxes and $n$ small boxes. You want to 'nest' them, represented by a sequence. `(` is a large box, `)` is a small box. A 'valid' nesting is a sequence like `(())` (small inside large, inside another large). How many different valid nesting combinations can you form with $n$ pairs?
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