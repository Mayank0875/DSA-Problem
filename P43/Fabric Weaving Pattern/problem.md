## Title
Fabric Weaving Pattern

## Slug
fabric-weaving-pattern

## Difficulty
Easy

## Description
A computerized loom uses a pattern string to control thread loops. There are three types of loops: `()`, `[]`, and `{}`. A valid pattern requires that every loop started must be completed, and loops cannot overlap in a way that tangles the thread (e.g., `([)]` causes a tangle). Given the design string, determine if the weaving pattern is physically possible without jamming the machine.

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
