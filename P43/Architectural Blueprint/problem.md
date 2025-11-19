## Title
Architectural Blueprint

## Slug
architectural-blueprint

## Difficulty
Easy

## Description
A CAD software exports a building's layout as a string. Buildings `{}`, Floors `[]`, and Rooms `()` are denoted by brackets. A valid blueprint must have rooms strictly inside floors, and floors strictly inside buildings. If a floor closes while a room is still undefined (open), the file is corrupt. Check the validity of the blueprint string.

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
