## Title
DNA Folding Simulation

## Slug
dna-folding-simulation

## Difficulty
Easy

## Description
Bioinformaticians predict protein shapes. The folding process is represented by brackets. Bonds must form without crossing strands in impossible ways.

A sequence is considered valid if:
    1. Every opening bond pair has a corresponding closing bond pair of the same type.
    2. bond pairs are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All bond pairs are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square bond pair `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
