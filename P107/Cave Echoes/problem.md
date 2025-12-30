## Title
Cave Echoes

## Slug
cave-echoes

## Difficulty
Easy

## Description
Sound waves bounce in a cave. An outgoing wave `(` creates a returning echo `)`.

The explorer has a sound recording represented by a string `s`. The string `s` is guaranteed to be a **natural echo** (a valid nested configuration).

However, interference cancels two waves. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a natural echo.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is natural echo.
- Removing the first `(` and last `)` leaves `()`, natural echo.
It is impossible to make it distorted.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a natural echo.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string distorted, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a natural echo.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

