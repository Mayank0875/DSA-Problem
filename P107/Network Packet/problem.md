## Title
Network Packet

## Slug
network-packet

## Difficulty
Easy

## Description
Data is encapsulated. A header `(` matches a footer `)`.

The admin has a data packet represented by a string `s`. The string `s` is guaranteed to be a **valid request** (a valid nested configuration).

However, packet loss drops two bytes. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a valid request.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is valid request.
- Removing the first `(` and last `)` leaves `()`, valid request.
It is impossible to make it corrupted.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a valid request.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string corrupted, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a valid request.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

