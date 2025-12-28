## Title
Russian Nesting Dolls

## Slug
russian-nesting-dolls

## Difficulty
Easy

## Description
A toy manufacturer makes intricate nesting dolls. Each doll type corresponds to a bracket pair. To package them correctly, every upper half must eventually meet its matching lower half in the right order.

A sequence is considered valid if:
    1. Every opening doll shell has a corresponding closing doll shell of the same type.
    2. doll shells are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All doll shells are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square doll shell `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
