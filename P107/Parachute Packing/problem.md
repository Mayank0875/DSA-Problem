## Title
Parachute Packing

## Slug
parachute-packing

## Difficulty
Easy

## Description
A parachute is folded in layers. A fold `(` is secured by a tuck `)`.

The skydiver has a packing sequence represented by a string `s`. The string `s` is guaranteed to be a **safe chute** (a valid nested configuration).

However, two folds come undone. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a safe chute.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is safe chute.
- Removing the first `(` and last `)` leaves `()`, safe chute.
It is impossible to make it tangled.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a safe chute.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string tangled, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a safe chute.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

