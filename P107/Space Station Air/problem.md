## Title
Space Station Air

## Slug
space-station-air

## Difficulty
Easy

## Description
Life support systems use cycling vents. An intake `(` is always paired with an exhaust `)`.

The astronaut has a ventilation log represented by a string `s`. The string `s` is guaranteed to be a **sealed system** (a valid nested configuration).

However, meteorite impact damages two vents. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a sealed system.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is sealed system.
- Removing the first `(` and last `)` leaves `()`, sealed system.
It is impossible to make it leaking.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a sealed system.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string leaking, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a sealed system.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

