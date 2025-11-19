## Title
Bank Vault Mechanism

## Slug
bank-vault-mechanism

## Difficulty
Easy

## Description
A bank vault has a time-lock mechanism with nested gears. Gear set A `()`, Gear set B `[]`, and Gear set C `{}`. To unlock, the inner gears must complete their rotation cycles (close) before the outer gears can complete theirs. Given the sequence of gear engagements, determine if the vault will open or jam.

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
