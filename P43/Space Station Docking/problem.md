## Title
Space Station Docking

## Slug
space-station-docking

## Difficulty
Easy

## Description
A space station has a series of airlocks. An outer airlock `[]` contains an inner airlock `()`, which might contain a decontamination chamber `{}`. Safety protocols demand that inner doors must cycle (open and close) completely before outer doors can be operated. Given a log of door operations, verify if the safety protocols were followed.

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
