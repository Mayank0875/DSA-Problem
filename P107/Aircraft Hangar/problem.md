## Title
Aircraft Hangar

## Slug
aircraft-hangar

## Difficulty
Easy

## Description
A hangar has massive nesting doors. The small personnel door must be secured before the medium vehicle door, and finally the main aircraft door.

A sequence is considered valid if:
    1. Every opening door mechanism has a corresponding closing door mechanism of the same type.
    2. door mechanisms are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All door mechanisms are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square door mechanism `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

## Input Format
- A single line containing a string s consisting only of the characters '(', ')', '{', '}', '[' and ']'

## Output Format
- Return true if the string is valid, and false otherwise.

## Constraints
- 1 ≤ length(s) ≤ 1e5
- s contains only characters '()', '[]', and '{}'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string
