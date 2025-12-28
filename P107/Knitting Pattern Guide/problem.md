## Title
Knitting Pattern Guide

## Slug
knitting-pattern-guide

## Difficulty
Easy

## Description
A knitting guide defines repeating stitch patterns. Nested repeats must be completed fully before moving to the next section of the scarf.

A sequence is considered valid if:
    1. Every opening stitch pattern has a corresponding closing stitch pattern of the same type.
    2. stitch patterns are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All stitch patterns are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square stitch pattern `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
