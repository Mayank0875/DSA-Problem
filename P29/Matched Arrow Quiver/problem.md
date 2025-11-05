## Title

Matched Arrow Quiver

## Slug

matched-arrow-quiver

## Difficulty

Easy

## Description

An archer has $n$ 'left-fletched' arrows and $n$ 'right-fletched' arrows. To be 'balanced', the archer must draw them from the quiver in a specific order. A sequence is 'balanced' if at no point has the archer drawn more 'right' arrows than 'left' arrows. How many balanced draw sequences are possible, assuming the last arrow drawn leaves an empty quiver?
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