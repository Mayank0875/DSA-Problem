## Title
Secure Tunnel System

## Slug
secure-tunnel-system

## Difficulty
Easy

## Description
A secret underground facility uses a series of security gates. There are three types of security zones, denoted by different bracket types. An opening bracket implies entering a zone, and a closing bracket implies leaving it. For security protocols to hold, you must leave the most recently entered zone before you can leave an outer zone. You are given a log of gate operations. Determine if the sequence represents a valid path where every entered zone is properly exited without any security breaches.

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
