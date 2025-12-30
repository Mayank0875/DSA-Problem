## Title
Submarine Hatch

## Slug
submarine-hatch

## Difficulty
Easy

## Description
Hatches are sealed. The outer door `(` locks with the inner door `)`.

The captain has a lock log represented by a string `s`. The string `s` is guaranteed to be a **watertight vessel** (a valid nested configuration).

However, two seals fail. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a watertight vessel.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is watertight vessel.
- Removing the first `(` and last `)` leaves `()`, watertight vessel.
It is impossible to make it flooded.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a watertight vessel.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string flooded, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a watertight vessel.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

