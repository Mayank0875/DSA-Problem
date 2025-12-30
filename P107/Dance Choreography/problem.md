## Title
Dance Choreography

## Slug
dance-choreography

## Difficulty
Easy

## Description
Dancers perform moves. A step forward `(` is mirrored by a step back `)`.

The choreographer has a routine represented by a string `s`. The string `s` is guaranteed to be a **fluid dance** (a valid nested configuration).

However, two dancers miss their cue. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a fluid dance.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is fluid dance.
- Removing the first `(` and last `)` leaves `()`, fluid dance.
It is impossible to make it off-beat.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a fluid dance.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string off-beat, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a fluid dance.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

