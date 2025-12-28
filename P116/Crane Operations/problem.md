## Title
Crane Operations

## Slug
crane-operations

## Difficulty
Medium

## Description
A crane moves loads. Each lift occupies a time slot.

The schedule has list of lifts, each defined by a start and an end, represented as a pair `[s, e]`.

The crane has one hook. A lift must finish strictly before the next begins. Specifically, to transition from lift `[a, b]` to a subsequent lift `[c, d]`, the e of the first lift must be **strictly less than** the s of the second lift (i.e., `b < c`).

You can select lifts in any order you like to form a valid work log. Your goal is to determine the maximum number of lifts that can be included in a single work log.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest work log is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The lifts can be reordered to form the work log `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available lifts.
- The next `n` lines each contain two integers, representing the `s` and `e` of an lift.

## Output Format
- Return a single integer representing the maximum length of the work log.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ s < e ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
