## Title
Suspension Bridge

## Slug
suspension-bridge

## Difficulty
Easy

## Description
Cables support the bridge deck. Left anchors `(` are paired with right anchors `)`.

The engineer has a cable layout represented by a string `s`. The string `s` is guaranteed to be a **stable bridge** (a valid nested configuration).

However, rust corrodes two anchors. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a stable bridge.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is stable bridge.
- Removing the first `(` and last `)` leaves `()`, stable bridge.
It is impossible to make it unsafe.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a stable bridge.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string unsafe, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a stable bridge.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

