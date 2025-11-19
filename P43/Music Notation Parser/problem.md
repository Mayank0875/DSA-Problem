## Title
Music Notation Parser

## Slug
music-notation-parser

## Difficulty
Easy

## Description
You are parsing a digital music sheet. The notation uses brackets to denote repeat bars, first/second endings, and phrasing. For the music to be readable, these markers must be balanced. You cannot end a phrase that hasn't started, and you must close an inner repeat loop before closing an outer one. Given the string of notation markers, verify if the sheet music syntax is correct.

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
