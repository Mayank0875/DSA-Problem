## Title
Magic Spell Ritual

## Slug
magic-spell-ritual

## Difficulty
Easy

## Description
A wizard performs a ritual involving nested magic circles. Each type of bracket represents a specific elemental circle. If a circle is not closed before the outer one ends, the spell fails.

A sequence is considered valid if:
    1. Every opening magic circle has a corresponding closing magic circle of the same type.
    2. magic circles are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All magic circles are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square magic circle `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
