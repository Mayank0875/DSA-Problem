## Title
Broken Keyboard Brackets

## Slug
broken-keyboard-brackets

## Difficulty
Easy

## Description
A computer science student has typed a long code block. The editor ensures the brackets are initially balanced.

The student has a code block represented by a string `s`. The string `s` is guaranteed to be a **balanced bracket sequence** (a valid nested configuration).

However, the keyboard malfunctions and backspaces randomly. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a balanced bracket sequence.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is balanced bracket sequence.
- Removing the first `(` and last `)` leaves `()`, balanced bracket sequence.
It is impossible to make it unbalanced.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a balanced bracket sequence.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string unbalanced, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a balanced bracket sequence.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

