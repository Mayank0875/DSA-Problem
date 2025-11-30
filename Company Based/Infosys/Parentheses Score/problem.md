## Title

Parentheses Score

## Slug

parentheses-score

## Difficulty

Medium

## Description

A data transmission protocol uses nested parentheses to structure packets. Your job is to calculate the 'value' of a transmitted packet, which is represented by a balanced parentheses string `s`. The value is calculated recursively: a basic packet `()` has a value of 1. A sequence of packets `AB` has a value equal to the sum of their individual values, `A + B`. A packet that encapsulates another packet, `(A)`, has a value of `2 * A`, where `A` is the value of the inner packet. Given the string `s`, calculate its total value.

## Examples

### 1

#### Input

()

#### Output

1

#### Explanation

Value of "()" = 1
    
### 2

#### Input

(())

#### Output

()

#### Explanation
This is `(A)` where `A = ()`. The score is `2 * Score(A)`, which is `2 * 1 = 2`.
  

## Input Format  

- The input consists of a single line containing the balanced parentheses string `s`.

## Output Format  

- Return single integer representing the total score of the string.
  

## Constraints  

- 1 ≤ s.length ≤ 50
- `s` consists of only `(` and `)`.
- `s` is a balanced parentheses string.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, recursion, string

## Companies
infosys