## Title
Nested Doll Organizer

## Slug
nested-doll-organizer

## Difficulty
Easy

## Description
You are organizing a display of traditional nesting dolls. There are three types of dolls, represented by parentheses, square brackets, and curly braces. An opening bracket represents the bottom half of a doll, and a closing bracket represents the top half. For the dolls to fit inside one another perfectly, every bottom half must be immediately followed by a matching top half or another smaller doll that is fully assembled. Given a sequence of doll halves, determine if they can be perfectly nested and closed.

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
