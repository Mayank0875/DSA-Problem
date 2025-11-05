## Title

Stock Market Fluctuations

## Slug

stock-market-fluctuations

## Difficulty

Easy

## Description

You are analyzing a simplified stock market. A 'tick' is either 'Up' or 'Down'. You are given $n$ 'Up' ticks and $n$ 'Down' ticks. A 'stable period' is a sequence of ticks that starts at a base price, never drops below that base price, and returns to the base price at the end. How many different 'stable periods' can be formed?
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