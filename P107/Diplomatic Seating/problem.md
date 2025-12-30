## Title
Diplomatic Seating

## Slug
diplomatic-seating

## Difficulty
Easy

## Description
Guests are seated at a round table. Every host `(` has a designated guest `)` next to them in a nested arrangement.

The diplomat has a seating chart represented by a string `s`. The string `s` is guaranteed to be a **polite arrangement** (a valid nested configuration).

However, two attendees cancel last minute. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a polite arrangement.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is polite arrangement.
- Removing the first `(` and last `)` leaves `()`, polite arrangement.
It is impossible to make it awkward.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a polite arrangement.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string awkward, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a polite arrangement.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

