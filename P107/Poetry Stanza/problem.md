## Title
Poetry Stanza

## Slug
poetry-stanza

## Difficulty
Easy

## Description
A poem follows a rhyme scheme. A rhyme A `(` matches another A `)`.

The poet has a verse represented by a string `s`. The string `s` is guaranteed to be a **rhyming couplet** (a valid nested configuration).

However, two words are smudged. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a rhyming couplet.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is rhyming couplet.
- Removing the first `(` and last `)` leaves `()`, rhyming couplet.
It is impossible to make it free verse.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a rhyming couplet.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string free verse, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a rhyming couplet.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

