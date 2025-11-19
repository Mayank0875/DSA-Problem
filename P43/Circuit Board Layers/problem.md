## Title
Circuit Board Layers

## Slug
circuit-board-layers

## Difficulty
Easy

## Description
A PCB design file describes layers of copper traces. Vias `()`, Pads `[]`, and Components `{}` are defined. Components contain pads, which contain vias. The manufacturing machine reads this nesting to drill holes. If the nesting is invalid (e.g., a component ends before its pad definition ends), the board will be ruined. Validate the design file.

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
