## Title
Game Level Design

## Slug
game-level-design

## Difficulty
Easy

## Description
A video game level is designed with nested zones. `()` are safe zones, `[]` are combat zones, and `{}` are boss arenas. Players must clear inner zones before leaving outer zones. If a player can exit a combat zone without clearing the inner safe zone first, the level design is flawed. Given the sequence of zone boundaries, determine if the level structure is valid.

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
