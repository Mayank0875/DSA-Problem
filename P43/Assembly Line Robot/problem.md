## Title
Assembly Line Robot

## Slug
assembly-line-robot

## Difficulty
Easy

## Description
An assembly line robot performs tasks grouped by priority. High priority `{}`, medium `[]`, and low `()`. A task group must be completed (closed) before returning to the outer task group. The robot logs a string of task initiations and completions. Analyze the log to determine if the robot followed the correct hierarchical operational procedure.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All opening brackets have matching closing brackets in the correct order.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The bracket '[' is closed by ')' which is a mismatch in type and nesting order.

## Input Format
- A single line containing a string s consisting only of the characters '(', ')', '{', '}', '[' and ']'.

## Output Format
- Return true (printed as Yes) if the string is valid, and false (printed as No) otherwise.

## Constraints
- 1 ≤ length(s) ≤ 1e5
- s contains only parentheses '()', square brackets '[]', and curly braces '{}'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string
