## Title
Map Contours Validator

## Slug
map-contours-validator

## Difficulty
Easy

## Description
A cartography software represents elevation contours using nested symbols. Different bracket types represent mountains, valleys, and plateaus. A valid map requires that a contour started within another contour must close before the outer contour closes (contours cannot cross). Given a string representing a slice of the map's topography, check if the geological representation is valid.

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
