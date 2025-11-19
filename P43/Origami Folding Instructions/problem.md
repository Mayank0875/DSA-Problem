## Title
Origami Folding Instructions

## Slug
origami-folding-instructions

## Difficulty
Easy

## Description
Origami diagrams use symbols to denote folds. Valley folds `()`, Mountain folds `[]`, and Reverse folds `{}`. Complex models involve steps nested within other steps. A valid instruction set requires that a specific folding sequence is completed before resuming the previous step. Check if the given string of folding steps is logically valid.

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
