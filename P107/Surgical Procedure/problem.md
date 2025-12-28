## Title
Surgical Procedure

## Slug
surgical-procedure

## Difficulty
Easy

## Description
A surgeon follows a protocol. An internal suture must be tied off before the external incision is closed.

A sequence is considered valid if:
    1. Every opening procedure step has a corresponding closing procedure step of the same type.
    2. procedure steps are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All procedure steps are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square procedure step `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
