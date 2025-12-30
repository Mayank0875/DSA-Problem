## Title
Traffic Tunnel

## Slug
traffic-tunnel

## Difficulty
Easy

## Description
Cars enter `(` and exit `)` a tunnel. The system tracks vehicle counts.

The controller has a sensor log represented by a string `s`. The string `s` is guaranteed to be a **clear tunnel** (a valid nested configuration).

However, sensors fail to detect two cars. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a clear tunnel.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is clear tunnel.
- Removing the first `(` and last `)` leaves `()`, clear tunnel.
It is impossible to make it congested.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a clear tunnel.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string congested, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a clear tunnel.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

