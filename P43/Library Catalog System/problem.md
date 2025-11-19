## Title
Library Catalog System

## Slug
library-catalog-system

## Difficulty
Easy

## Description
A library organizes materials by Collection `{}`, Shelf `[]`, and Book `()`. The digital catalog represents this hierarchy as a string. A catalog entry is invalid if a Shelf is marked as 'end' while a Book entry is still 'open'. You are given the structure string of a section of the library. Verify if the catalog organization is error-free.

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
