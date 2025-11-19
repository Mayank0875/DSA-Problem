## Title
Inventory Package Nesting

## Slug
inventory-package-nesting

## Difficulty
Easy

## Description
An inventory robot packs items into boxes `[]`, bags `()`, and crates `{}`. Items can be nested (e.g., a bag inside a box). The robot scans the items as it packs (open bracket) and seals (close bracket) them. A packing error occurs if the robot tries to seal a crate while a bag inside it is still open. Given the scan log, determine if the packing process was performed correctly.

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
