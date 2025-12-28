## Title
Robot Path Loop

## Slug
robot-path-loop

## Difficulty
Easy

## Description
A rover explores Mars using command loops. Instructions use brackets to define start and end points of exploration zones. Loops must not overlap incorrectly.

A sequence is considered valid if:
    1. Every opening command loop has a corresponding closing command loop of the same type.
    2. command loops are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All command loops are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square command loop `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
