## Title
Bank Vault Security

## Slug
bank-vault-security

## Difficulty
Easy

## Description
A high-security vault has layers of time-locked doors. An inner door sequence must complete its cycle before the outer door sequence can proceed.

A sequence is considered valid if:
    1. Every opening security door has a corresponding closing security door of the same type.
    2. security doors are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All security doors are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square security door `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
