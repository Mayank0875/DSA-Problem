## Title
Ancient Pottery

## Slug
ancient-pottery

## Difficulty
Easy

## Description
A clay pot is formed. The convex curve `(` meets a concave curve `)`.

The archaeologist has a pot shape represented by a string `s`. The string `s` is guaranteed to be a **intact artifact** (a valid nested configuration).

However, time erodes two shards. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a intact artifact.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is intact artifact.
- Removing the first `(` and last `)` leaves `()`, intact artifact.
It is impossible to make it broken.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a intact artifact.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string broken, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a intact artifact.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

