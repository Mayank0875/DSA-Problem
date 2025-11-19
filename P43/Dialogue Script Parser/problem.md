## Title
Dialogue Script Parser

## Slug
dialogue-script-parser

## Difficulty
Easy

## Description
A scriptwriting software uses brackets to annotate text: `()` for actions, `[]` for scene descriptions, and `{}` for character emotions. The software needs to ensure that no annotation is left unclosed and that they don't overlap incorrectly (e.g., an action starts inside an emotion but doesn't end there). Given the annotation string, verify if the script format is valid.

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
