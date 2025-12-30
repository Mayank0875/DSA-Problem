## Title
Piano Tuning

## Slug
piano-tuning

## Difficulty
Easy

## Description
Strings are tightened. Tension `(` is balanced by the frame `)`.

The tuner has a string set represented by a string `s`. The string `s` is guaranteed to be a **tuned piano** (a valid nested configuration).

However, two strings snap. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a tuned piano.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is tuned piano.
- Removing the first `(` and last `)` leaves `()`, tuned piano.
It is impossible to make it dissonant.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a tuned piano.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string dissonant, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a tuned piano.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

