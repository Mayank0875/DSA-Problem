## Title
Safe Lock Sequence

## Slug
safe-lock-sequence

## Difficulty
Easy

## Description
A sophisticated electronic safe requires a sequence of key turns to open. There are three tumblers, represented by different bracket pairs. Turning a key 'open' corresponds to an open bracket, and 'close' to a closed bracket. The mechanism jams if you try to close a tumbler that wasn't the most recently opened one. Given a sequence of key turns, determine if the sequence will successfully operate the lock without jamming.

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
