## Title
Warehouse Boxes

## Slug
warehouse-boxes

## Difficulty
Easy

## Description
Boxes are stacked inside larger boxes. The arrangement is verified to be physically possible.

The manager has a box stack represented by a string `s`. The string `s` is guaranteed to be a **nested shipment** (a valid nested configuration).

However, two boxes are damaged and removed. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a nested shipment.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is nested shipment.
- Removing the first `(` and last `)` leaves `()`, nested shipment.
It is impossible to make it invalid stack.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a nested shipment.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string invalid stack, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a nested shipment.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

