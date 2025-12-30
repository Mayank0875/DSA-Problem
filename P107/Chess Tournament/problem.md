## Title
Chess Tournament

## Slug
chess-tournament

## Difficulty
Easy

## Description
Players are paired. White `(` plays against Black `)`.

The arbiter has a match list represented by a string `s`. The string `s` is guaranteed to be a **fair round** (a valid nested configuration).

However, two players withdraw. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a fair round.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is fair round.
- Removing the first `(` and last `)` leaves `()`, fair round.
It is impossible to make it uneven.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a fair round.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string uneven, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a fair round.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

