## Title
Cargo Ship Stability

## Slug
cargo-ship-stability

## Difficulty
Easy

## Description
A loadmaster balances a ship. Securing a block of cargo requires specific lashings (brackets). Inner lashings must be tight before outer straps are applied.

A sequence is considered valid if:
    1. Every opening lashing group has a corresponding closing lashing group of the same type.
    2. lashing groups are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All lashing groups are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square lashing group `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

## Input Format
- A single line containing a string s consisting only of the characters '(', ')', '{', '}', '[' and ']'

## Output Format
- Return true if the string is valid, and false otherwise.

## Constraints
- 1 ≤ length(s) ≤ 1e5
- s contains only characters '()', '[]', and '{}'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string
