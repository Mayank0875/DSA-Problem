## Title
Programming Macro Expansion

## Slug
programming-macro-expansion

## Difficulty
Easy

## Description
A pre-processor expands macros in C code. Macros use parentheses, but the code blocks they generate use braces and array indices use brackets. If a macro expands incorrectly, it might produce code with mismatched delimiters. You are given the delimiter sequence of an expanded macro. Determine if the resulting code has valid syntax.

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
