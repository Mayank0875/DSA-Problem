## Title
Train Cargo Configuration

## Slug
train-cargo-configuration

## Difficulty
Easy

## Description
A freight train is loaded with containers `[]`, which contain pallets `{}`, which contain boxes `()`. The loading manifest records the start and end of each storage unit. For the cargo to be secure, every unit must be fully enclosed within its parent unit without any crossover. Given the manifest string, determine if the cargo loading configuration is valid.

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
