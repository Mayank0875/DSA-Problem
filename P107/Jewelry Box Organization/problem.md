## Title
Jewelry Box Organization

## Slug
jewelry-box-organization

## Difficulty
Easy

## Description
A luxury organizer has compartments inside compartments. You verify that every lid is closed on the correct box before closing the larger box containing it.

A sequence is considered valid if:
    1. Every opening compartment has a corresponding closing compartment of the same type.
    2. compartments are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All compartments are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square compartment `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
