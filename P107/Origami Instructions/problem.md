## Title
Origami Instructions

## Slug
origami-instructions

## Difficulty
Easy

## Description
An origami book describes folds. A complex fold sequence involves opening a flap, making internal folds, and closing it back up.

A sequence is considered valid if:
    1. Every opening fold sequence has a corresponding closing fold sequence of the same type.
    2. fold sequences are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All fold sequences are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square fold sequence `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
