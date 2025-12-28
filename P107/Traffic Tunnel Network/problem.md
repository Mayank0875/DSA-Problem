## Title
Traffic Tunnel Network

## Slug
traffic-tunnel-network

## Difficulty
Easy

## Description
A city has a complex tunnel system. Entering a sub-tunnel implies you must exit it before you can exit the main highway tunnel.

A sequence is considered valid if:
    1. Every opening tunnel segment has a corresponding closing tunnel segment of the same type.
    2. tunnel segments are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All tunnel segments are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square tunnel segment `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
