## Title
Chemical Molecule Balancer

## Slug
chemical-molecule-balancer

## Difficulty
Easy

## Description
A chemist needs a tool to check if chemical formulas are structurally sound. Groups of atoms denoted by different types of brackets must be closed correctly to form stable molecules.

A sequence is considered valid if:
    1. Every opening chemical group has a corresponding closing chemical group of the same type.
    2. chemical groups are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All chemical groups are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square chemical group `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
