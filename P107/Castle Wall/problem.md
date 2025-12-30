## Title
Castle Wall

## Slug
castle-wall

## Difficulty
Easy

## Description
Stones are laid. A stone `(` supports another `)`.

The mason has a wall section represented by a string `s`. The string `s` is guaranteed to be a **fortified wall** (a valid nested configuration).

However, a siege engine knocks out two stones. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a fortified wall.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is fortified wall.
- Removing the first `(` and last `)` leaves `()`, fortified wall.
It is impossible to make it breached.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a fortified wall.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string breached, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a fortified wall.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

