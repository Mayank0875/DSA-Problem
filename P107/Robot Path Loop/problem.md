## Title
Robot Path Loop

## Slug
robot-path-loop

## Difficulty
Easy

## Description
A robot follows a path of loops. Entering a loop `(` must eventually lead to exiting it `)`.

The engineer has a path log represented by a string `s`. The string `s` is guaranteed to be a **closed loop system** (a valid nested configuration).

However, data corruption deletes two commands. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a closed loop system.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is closed loop system.
- Removing the first `(` and last `)` leaves `()`, closed loop system.
It is impossible to make it open-ended.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a closed loop system.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string open-ended, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a closed loop system.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

