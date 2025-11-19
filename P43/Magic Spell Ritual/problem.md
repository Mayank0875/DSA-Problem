## Title
Magic Spell Ritual

## Slug
magic-spell-ritual

## Difficulty
Easy

## Description
A wizard casts a spell involving nested magic circles. `()` represents a protection circle, `[]` a summoning circle, and `{}` a binding circle. For the spell to work without backfiring, circles must be drawn and closed in a strict LIFO (Last-In, First-Out) order. Given the sequence of circle drawings, determine if the spell will be cast successfully.

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
