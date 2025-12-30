## Title
Jewelry Chain

## Slug
jewelry-chain

## Difficulty
Easy

## Description
A jeweler inspects a gold chain. The links are formed in pairs to create a specific pattern.

The jeweler has a chain link pattern represented by a string `s`. The string `s` is guaranteed to be a **intact chain** (a valid nested configuration).

However, two links are removed for resizing. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a intact chain.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is intact chain.
- Removing the first `(` and last `)` leaves `()`, intact chain.
It is impossible to make it tangled.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a intact chain.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string tangled, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a intact chain.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

