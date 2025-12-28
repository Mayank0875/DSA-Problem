## Title
Train Marshaling

## Slug
train-marshaling

## Difficulty
Easy

## Description
Train cars are coupled in specific blocks. A block of cars started with a specific engine type must be ended with a matching caboose type before a larger block ends.

A sequence is considered valid if:
    1. Every opening car block has a corresponding closing car block of the same type.
    2. car blocks are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All car blocks are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square car block `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
