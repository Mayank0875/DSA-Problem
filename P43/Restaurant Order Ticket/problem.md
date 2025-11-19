## Title
Restaurant Order Ticket

## Slug
restaurant-order-ticket

## Difficulty
Easy

## Description
A kitchen display system groups orders. Tables are `{}`, Seats are `[]`, and Courses are `()`. An order ticket string is generated. A valid ticket must have courses nested in seats, and seats nested in tables, without any overlap. Check if the generated ticket string represents a valid grouping of a meal order.

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
