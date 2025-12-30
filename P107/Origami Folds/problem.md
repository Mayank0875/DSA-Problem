## Title
Origami Folds

## Slug
origami-folds

## Difficulty
Easy

## Description
Paper is folded into art. A valley fold `(` is matched by a mountain fold `)`.

The artist has a fold list represented by a string `s`. The string `s` is guaranteed to be a **symmetric crane** (a valid nested configuration).

However, the paper tears at two spots. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a symmetric crane.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is symmetric crane.
- Removing the first `(` and last `)` leaves `()`, symmetric crane.
It is impossible to make it ruined.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a symmetric crane.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string ruined, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a symmetric crane.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

