## Title
Network Packet Encapsulation

## Slug
network-packet-encapsulation

## Difficulty
Easy

## Description
In network transmission, data is encapsulated in headers and footers. We visualize different protocols (TCP, UDP, HTTP) as different bracket pairs. A packet is valid if every protocol header has a matching footer and the encapsulation is strictly nested (Layer 4 inside Layer 3, etc.). Given a string representing the sequence of headers (openers) and footers (closers), determine if the packet is malformed.

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
