## Title
Tax Audit

## Slug
tax-audit

## Difficulty
Easy

## Description
Expenses are filed. A deduction `(` must be supported by a receipt `)`.

The auditor has a tax return represented by a string `s`. The string `s` is guaranteed to be a **compliant filing** (a valid nested configuration).

However, two receipts are lost. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a compliant filing.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is compliant filing.
- Removing the first `(` and last `)` leaves `()`, compliant filing.
It is impossible to make it audited.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a compliant filing.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string audited, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a compliant filing.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

