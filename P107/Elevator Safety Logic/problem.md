## Title
Elevator Safety Logic

## Slug
elevator-safety-logic

## Difficulty
Easy

## Description
An elevator controller manages door safety. The inner doors must close fully before the outer floor doors lock. A glitch occurs if they cross signals.

A sequence is considered valid if:
    1. Every opening door cycle has a corresponding closing door cycle of the same type.
    2. door cycles are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All door cycles are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square door cycle `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
