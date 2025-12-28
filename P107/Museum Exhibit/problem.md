## Title
Museum Exhibit

## Slug
museum-exhibit

## Difficulty
Easy

## Description
Artifacts are placed in cases. A small relic goes in a small case, which goes inside a larger climate-controlled display. The cases must be sealed in order.

A sequence is considered valid if:
    1. Every opening display case has a corresponding closing display case of the same type.
    2. display cases are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All display cases are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square display case `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
