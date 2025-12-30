## Title
Magic Spell Syntax

## Slug
magic-spell-syntax

## Difficulty
Easy

## Description
A wizard casts a complex spell. The incantations must be nested correctly to contain the magical energy.

The wizard has a spell scroll represented by a string `s`. The string `s` is guaranteed to be a **safe spell** (a valid nested configuration).

However, a stutter causes two runes to vanish. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a safe spell.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is safe spell.
- Removing the first `(` and last `)` leaves `()`, safe spell.
It is impossible to make it volatile.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a safe spell.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string volatile, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a safe spell.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

