## Title
Network Packet Encapsulation

## Slug
network-packet-encapsulation

## Difficulty
Easy

## Description
Data travels the internet inside layers of protocols (headers/footers). A router checks if the packet layers are stripped in the correct reverse order of their addition.

A sequence is considered valid if:
    1. Every opening protocol layer has a corresponding closing protocol layer of the same type.
    2. protocol layers are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All protocol layers are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square protocol layer `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
