## Title
Book Chapter Organization

## Slug
book-chapter-organization

## Difficulty
Easy

## Description
An e-book format uses brackets to define the hierarchy of Parts `{}`, Chapters `[]`, and Sections `()`. The formatting engine requires that these sections be strictly nested; a Chapter cannot end if a Section inside it is still open. You are given a string representing the structure tags of a book. Verify if the book's structure is valid for publishing.

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
