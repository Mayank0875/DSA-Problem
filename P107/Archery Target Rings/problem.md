## Title
Archery Target Rings

## Slug
archery-target-rings

## Difficulty
Easy

## Description
An archery target consists of concentric rings. Each inner ring is enclosed by an outer ring.

The archer has a target pattern represented by a string `s`. The string `s` is guaranteed to be a **valid target** (a valid nested configuration).

However, two rings are removed for maintenance. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a valid target.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is valid target.
- Removing the first `(` and last `)` leaves `()`, valid target.
It is impossible to make it defective.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a valid target.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string defective, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a valid target.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

