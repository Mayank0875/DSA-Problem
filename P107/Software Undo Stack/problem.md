## Title
Software Undo Stack

## Slug
software-undo-stack

## Difficulty
Easy

## Description
A text editor tracks changes. A 'macro' action groups multiple edits. The undo system verifies that macros are closed properly before saving history.

A sequence is considered valid if:
    1. Every opening edit group has a corresponding closing edit group of the same type.
    2. edit groups are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All edit groups are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square edit group `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
