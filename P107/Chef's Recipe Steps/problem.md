## Title
Chef's Recipe Steps

## Slug
chefs-recipe-steps

## Difficulty
Easy

## Description
A recipe has nested instructions (e.g., 'while the sauce simmers, chop onions'). You must finish the inner task before completing the outer cooking phase.

A sequence is considered valid if:
    1. Every opening cooking task has a corresponding closing cooking task of the same type.
    2. cooking tasks are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All cooking tasks are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square cooking task `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
