## Title
HTML Tag Cleaner

## Slug
html-tag-cleaner

## Difficulty
Easy

## Description
A web scraper parses HTML tags. The document is strictly valid with opening and closing tags.

The developer has a tag sequence represented by a string `s`. The string `s` is guaranteed to be a **valid DOM** (a valid nested configuration).

However, a parser error drops two tags. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a valid DOM.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is valid DOM.
- Removing the first `(` and last `)` leaves `()`, valid DOM.
It is impossible to make it broken HTML.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a valid DOM.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string broken HTML, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a valid DOM.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

