## Title
Lisp Code Validator

## Slug
lisp-code-validator

## Difficulty
Easy

## Description
You are working on an interpreter for a Lisp-like language that heavily relies on nested lists. While the original language uses only parentheses, this dialect uses square brackets and curly braces for specific data structures. The interpreter crashes if the nesting is incorrect. Your task is to write a pre-check routine that takes the sequence of brackets from the source code and returns whether the nesting structure is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All opening brackets have matching closing brackets in the correct order.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The bracket '[' is closed by ')' which is a mismatch in type and nesting order.

## Input Format
- A single line containing a string s consisting only of the characters '(', ')', '{', '}', '[' and ']'.

## Output Format
- Return true (printed as Yes) if the string is valid, and false (printed as No) otherwise.

## Constraints
- 1 ≤ length(s) ≤ 1e5
- s contains only parentheses '()', square brackets '[]', and curly braces '{}'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string
