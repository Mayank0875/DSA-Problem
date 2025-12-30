## Title
Train Coupling

## Slug
train-coupling

## Difficulty
Easy

## Description
A train is assembled with specific coupling hooks. Every front hook `(` is met with a rear hook `)`.

The conductor has a train assembly represented by a string `s`. The string `s` is guaranteed to be a **coupled train** (a valid nested configuration).

However, a mechanical failure breaks two couplers. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a coupled train.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is coupled train.
- Removing the first `(` and last `)` leaves `()`, coupled train.
It is impossible to make it uncoupled.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a coupled train.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string uncoupled, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a coupled train.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

