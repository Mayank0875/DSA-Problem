## Title
Library Bookshelf

## Slug
library-bookshelf

## Difficulty
Easy

## Description
Books are held by bookends. A left bookend `(` matches a right bookend `)`.

The librarian has a shelf arrangement represented by a string `s`. The string `s` is guaranteed to be a **upright books** (a valid nested configuration).

However, two bookends slide off. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a upright books.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is upright books.
- Removing the first `(` and last `)` leaves `()`, upright books.
It is impossible to make it toppled.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a upright books.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string toppled, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a upright books.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

