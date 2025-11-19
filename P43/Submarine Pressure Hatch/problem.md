## Title
Submarine Pressure Hatch

## Slug
submarine-pressure-hatch

## Difficulty
Easy

## Description
A submarine has nested pressure compartments. The hull `{}`, the ballast tanks `[]`, and the airlock `()`. Sensors record the pressurization (open) and depressurization (close) of these compartments. For structural integrity, an inner compartment must depressurize before the outer one does. Given the sensor log, determine if the submarine operations are safe.

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
