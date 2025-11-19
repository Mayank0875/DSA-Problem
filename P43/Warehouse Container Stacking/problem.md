## Title
Warehouse Container Stacking

## Slug
warehouse-container-stacking

## Difficulty
Easy

## Description
A shipping company uses three types of containers that can be placed inside one another. We represent the opening of a container with an opening bracket and the sealing of a container with a closing bracket. For a shipment to be valid, every container opened must be sealed with the correct lid, and no container can be sealed if an inner container is still open. Given the loading sequence, determine if the shipment configuration is valid.

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
