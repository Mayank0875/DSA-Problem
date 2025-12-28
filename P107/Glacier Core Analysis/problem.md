## Title
Glacier Core Analysis

## Slug
glacier-core-analysis

## Difficulty
Easy

## Description
Scientists drill ice cores. Layers of ice represent years. An anomaly within a year must be resolved before the year's data block is marked complete.

A sequence is considered valid if:
    1. Every opening ice layer has a corresponding closing ice layer of the same type.
    2. ice layers are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All ice layers are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square ice layer `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
