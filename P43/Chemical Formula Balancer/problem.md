## Title
Chemical Formula Balancer

## Slug
chemical-formula-balancer

## Difficulty
Easy

## Description
In a chemistry lab software, complex molecular structures are represented using various brackets to denote nested functional groups. Parentheses, square brackets, and curly braces represent different levels of molecular bonding. To ensure the formula is chemically possible, the software checks if the brackets are balanced and properly nested. You are given a string representing the bracket structure of a molecule. Your task is to determine if the structural representation is valid.

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
