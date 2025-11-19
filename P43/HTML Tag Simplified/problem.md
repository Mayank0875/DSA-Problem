## Title
HTML Tag Simplified

## Slug
html-tag-simplified

## Difficulty
Easy

## Description
You are writing a parser for a simplified markup language. Instead of full tags like `<div>`, this language uses brackets `()`, `[]`, and `{}` to define elements. A document is considered well-formed if every element that is opened is eventually closed, and elements are strictly nested (an element opened inside another must close before the outer one). Given a string of these characters representing the document structure, check if it is well-formed.

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
