## Title
Alien Signal Decoder

## Slug
alien-signal-decoder

## Difficulty
Easy

## Description
SETI researchers have received a signal containing pairs of distinct frequency modulations represented by brackets. They believe the signal represents a hierarchical language. For the message to be intelligible, the modulation pairs must be balanced and nested correctly, similar to mathematical syntax. You are given the signal string. Your task is to determine if the signal is a valid construct or just random noise.

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
