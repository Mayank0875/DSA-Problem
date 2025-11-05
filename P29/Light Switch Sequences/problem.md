## Title

Light Switch Sequences

## Slug

light-switch-sequences

## Difficulty

Easy

## Description

A light switch starts in the 'Off' state. You have $n$ 'On' flicks and $n$ 'Off' flicks. A 'valid' sequence of flicks is one that never tries to turn the light 'Off' when it is already off, and ends with the light 'Off'. How many different valid sequences can be formed using exactly $n$ 'On' and $n$ 'Off' flicks?
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