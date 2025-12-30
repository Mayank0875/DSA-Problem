## Title
Battery Stack

## Slug
battery-stack

## Difficulty
Easy

## Description
Batteries are arranged in a pack. Positive terminals `(` align with negative terminals `)`.

The technician has a battery pack represented by a string `s`. The string `s` is guaranteed to be a **powered circuit** (a valid nested configuration).

However, two terminals corrode. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a powered circuit.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is powered circuit.
- Removing the first `(` and last `)` leaves `()`, powered circuit.
It is impossible to make it dead.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a powered circuit.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string dead, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a powered circuit.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

