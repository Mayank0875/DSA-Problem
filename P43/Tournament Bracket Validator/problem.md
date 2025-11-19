## Title
Tournament Bracket Validator

## Slug
tournament-bracket-validator

## Difficulty
Easy

## Description
You are managing an e-sports tournament. The match structure is complex, involving Groups `{}`, Matches `[]`, and Rounds `()`. The tournament software generates a string representing the bracket structure. You must validate this string to ensure that every round ends within its match, and every match ends within its group. Is the bracket valid?

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
