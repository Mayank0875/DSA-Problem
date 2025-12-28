## Title
Deep Sea Submarine

## Slug
deep-sea-submarine

## Difficulty
Easy

## Description
A submarine descends into a trench. Pressure chambers (brackets) activate to protect the hull. They must be deactivated in the correct order during ascent.

A sequence is considered valid if:
    1. Every opening pressure chamber has a corresponding closing pressure chamber of the same type.
    2. pressure chambers are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All pressure chambers are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square pressure chamber `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
