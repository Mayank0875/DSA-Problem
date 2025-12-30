## Title
Theater Curtains

## Slug
theater-curtains

## Difficulty
Easy

## Description
Stage curtains consist of layers. Each opening drape `(` has a closing drape `)`.

The stage manager has a curtain rig represented by a string `s`. The string `s` is guaranteed to be a **hidden stage** (a valid nested configuration).

However, a mechanism jams two drapes. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a hidden stage.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is hidden stage.
- Removing the first `(` and last `)` leaves `()`, hidden stage.
It is impossible to make it exposed.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a hidden stage.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string exposed, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a hidden stage.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

