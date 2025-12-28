## Title
Telescope Assembly

## Slug
telescope-assembly

## Difficulty
Easy

## Description
A space telescope unfolds its mirrors. The deployment mechanism has nested stages. Stage B must fully deploy and lock before Stage A can continue.

A sequence is considered valid if:
    1. Every opening deployment stage has a corresponding closing deployment stage of the same type.
    2. deployment stages are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All deployment stages are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square deployment stage `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
