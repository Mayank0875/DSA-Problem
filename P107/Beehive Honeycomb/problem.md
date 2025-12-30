## Title
Beehive Honeycomb

## Slug
beehive-honeycomb

## Difficulty
Easy

## Description
Bees build cells. A wax wall `(` connects to another `)`.

The beekeeper has a comb structure represented by a string `s`. The string `s` is guaranteed to be a **strong hive** (a valid nested configuration).

However, a bear damages two walls. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a strong hive.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is strong hive.
- Removing the first `(` and last `)` leaves `()`, strong hive.
It is impossible to make it collapsed.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a strong hive.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string collapsed, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a strong hive.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

