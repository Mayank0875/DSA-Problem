## Title
Space Station Airlocks

## Slug
space-station-airlocks

## Difficulty
Easy

## Description
An automated system controls the airlocks of a space station. Nested zones use different security protocols (brackets). An inner airlock cannot be left open if the outer one is closing.

A sequence is considered valid if:
    1. Every opening airlock door has a corresponding closing airlock door of the same type.
    2. airlock doors are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All airlock doors are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square airlock door `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
