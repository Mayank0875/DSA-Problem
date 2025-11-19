## Title
JSON Format Checker

## Slug
json-format-checker

## Difficulty
Easy

## Description
You are validating JSON-like data strings which consist of objects `{}` and arrays `[]`. Sometimes, comments are encapsulated in `()`. A valid data string must have every object, array, and comment properly closed and nested. You extract just the structural characters from a data file. Your task is to determine if this extracted sequence represents a valid data structure where all openers match their closers in the correct order.

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
