## Title
Warehouse Container Loading

## Slug
warehouse-container-loading

## Difficulty
Easy

## Description
A logistics robot loads containers. Different bracket types represent different container sizes. A container can only be closed if all smaller containers inside it have been fully closed first.

A sequence is considered valid if:
    1. Every opening container has a corresponding closing container of the same type.
    2. containers are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All containers are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square container `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
