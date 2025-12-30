## Title
Fence Post

## Slug
fence-post

## Difficulty
Easy

## Description
A fence is built. A post `(` supports a panel `)`.

The builder has a fence line represented by a string `s`. The string `s` is guaranteed to be a **standing fence** (a valid nested configuration).

However, a storm knocks down two parts. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a standing fence.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is standing fence.
- Removing the first `(` and last `)` leaves `()`, standing fence.
It is impossible to make it gapped.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a standing fence.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string gapped, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a standing fence.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

