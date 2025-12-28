## Title
Assembly Line Robot

## Slug
assembly-line-robot

## Difficulty
Easy

## Description
A robot assembles cars. It picks up parts (opening) and installs them (closing). It cannot install a larger outer part until the inner parts are secured.

A sequence is considered valid if:
    1. Every opening assembly step has a corresponding closing assembly step of the same type.
    2. assembly steps are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All assembly steps are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square assembly step `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
