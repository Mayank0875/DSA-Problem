## Title
Legal Document Review

## Slug
legal-document-review

## Difficulty
Easy

## Description
An AI reviews contracts. Clauses are often nested within other clauses. The AI checks if every sub-clause is properly terminated within its parent section.

A sequence is considered valid if:
    1. Every opening clause has a corresponding closing clause of the same type.
    2. clauses are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All clauses are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square clause `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

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
