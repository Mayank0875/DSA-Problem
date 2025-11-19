## Title
Mathematical Expression Checker

## Slug
mathematical-expression-checker

## Difficulty
Easy

## Description
You are designing a calculator app that accepts complex mathematical expressions. Users can use parentheses, square brackets, and curly braces to group operations. Before evaluating the expression, the app must ensure the grouping is valid. A valid expression requires that every open bracket has a matching closed bracket of the same type and that nested groups are closed correctly. Given a string of these characters representing the structure of the equation, determine if the expression is valid.

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
