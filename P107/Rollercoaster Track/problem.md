## Title
Rollercoaster Track

## Slug
rollercoaster-track

## Difficulty
Easy

## Description
The track loops. An ascent `(` is followed by a descent `)`.

The rider has a track layout represented by a string `s`. The string `s` is guaranteed to be a **thrilling ride** (a valid nested configuration).

However, maintenance removes two sections. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a thrilling ride.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is thrilling ride.
- Removing the first `(` and last `)` leaves `()`, thrilling ride.
It is impossible to make it dangerous.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a thrilling ride.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string dangerous, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a thrilling ride.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

