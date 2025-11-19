## Title
Algebraic Grouping Check

## Slug
algebraic-grouping-check

## Difficulty
Easy

## Description
A math tutor application checks student homework. The students input complicated algebraic expressions involving multiple layers of grouping. The most common error is mismatched or misplaced brackets. You are given the skeleton of the expression containing only the grouping symbols. Your task is to determine if the student has grouped the terms correctly.

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
