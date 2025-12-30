## Title
Circuit Logic

## Slug
circuit-logic

## Difficulty
Easy

## Description
An electrician wires a circuit. Nested sub-circuits must be closed properly to function.

The electrician has a wiring diagram represented by a string `s`. The string `s` is guaranteed to be a **short-free circuit** (a valid nested configuration).

However, a wire snaps at two points. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a short-free circuit.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is short-free circuit.
- Removing the first `(` and last `)` leaves `()`, short-free circuit.
It is impossible to make it short-circuited.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a short-free circuit.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string short-circuited, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a short-free circuit.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

