## Title
Inventory Audit

## Slug
inventory-audit

## Difficulty
Easy

## Description
Items are checked in `(` and checked out `)`. The inventory count is balanced at the end of the day.

The auditor has a audit log represented by a string `s`. The string `s` is guaranteed to be a **balanced inventory** (a valid nested configuration).

However, two records are lost. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a balanced inventory.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is balanced inventory.
- Removing the first `(` and last `)` leaves `()`, balanced inventory.
It is impossible to make it discrepant.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a balanced inventory.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string discrepant, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a balanced inventory.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

