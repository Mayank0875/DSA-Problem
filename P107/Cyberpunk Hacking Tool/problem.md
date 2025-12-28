## Title
Cyberpunk Hacking Tool

## Slug
cyberpunk-hacking-tool

## Difficulty
Easy

## Description
A hacker breaches ICE (Intrusion Countermeasures Electronics). Nested firewalls must be deactivated from the inside out to avoid detection.

A sequence is considered valid if:
    1. Every opening firewall layer has a corresponding closing firewall layer of the same type.
    2. firewall layers are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All firewall layers are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square firewall layer `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
