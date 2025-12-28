## Title
Parachute Packing

## Slug
parachute-packing

## Difficulty
Easy

## Description
A skydiver packs a chute. The pilot chute is folded inside the main canopy, which is folded inside the container. The packing order must be strictly valid.

A sequence is considered valid if:
    1. Every opening fold layer has a corresponding closing fold layer of the same type.
    2. fold layers are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All fold layers are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square fold layer `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
