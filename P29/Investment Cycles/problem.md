## Title

Investment Cycles

## Slug

investment-cycles

## Difficulty

Easy

## Description

You are modeling $n$ investment cycles. Each cycle has an 'Invest' action and a 'Divest' action. A 'prudent' history of actions is a sequence where you never 'Divest' unless you have an 'Invest' to match it, and all investments are eventually divested. How many different prudent histories are there?
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