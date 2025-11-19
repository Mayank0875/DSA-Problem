## Title
Code Syntax Validator

## Slug
code-syntax-validator

## Difficulty
Easy

## Description
You are building a lightweight code editor for a programming competition. One of the essential features is a syntax checker that ensures all code blocks are properly closed. The code snippet is simplified into a string containing only grouping symbols: parentheses, square brackets, and curly braces. For the code to be valid, every opening symbol must be closed by the same type, and they must be closed in the reverse order they were opened (LIFO). Your task is to verify if the given sequence of brackets represents a syntactically correct code structure.

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
