## Title
Telescope Lens Setup

## Slug
telescope-lens-setup

## Difficulty
Easy

## Description
An optical engineer arranges lenses in a tube. There are different lens holders: `()`, `[]`, and `{}`. A holder can contain other smaller holders. For the telescope to focus, the holders must be placed such that inner holders are secured before outer holders are sealed. Given the assembly arrangement string, verify if the lens setup is mechanically valid.

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
