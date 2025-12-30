## Title
Secure Tunnel System

## Slug
secure-tunnel-system

## Difficulty
Easy

## Description
A high-security facility uses airlock gates. Opening an entry gate `(` requires a corresponding exit gate `)`.

The security chief has a gate log represented by a string `s`. The string `s` is guaranteed to be a **secure sequence** (a valid nested configuration).

However, a system glitch forces two gates to malfunction. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a secure sequence.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is secure sequence.
- Removing the first `(` and last `)` leaves `()`, secure sequence.
It is impossible to make it breached.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a secure sequence.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string breached, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a secure sequence.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

