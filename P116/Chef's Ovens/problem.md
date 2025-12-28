## Title
Chef's Ovens

## Slug
chefs-ovens

## Difficulty
Medium

## Description
A chef schedules baking. Each dish needs the oven for a time interval.

The menu has list of dishes, each defined by a in time and an out time, represented as a pair `[in, out]`.

There is only one oven. A dish must come out strictly before the next one goes in. Specifically, to transition from dish `[a, b]` to a subsequent dish `[c, d]`, the out of the first dish must be **strictly less than** the in of the second dish (i.e., `b < c`).

You can select dishes in any order you like to form a valid baking schedule. Your goal is to determine the maximum number of dishes that can be included in a single baking schedule.

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
The longest baking schedule is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The dishes can be reordered to form the baking schedule `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available dishes.
- The next `n` lines each contain two integers, representing the `in` and `out` of an dish.

## Output Format
- Return a single integer representing the maximum length of the baking schedule.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ in < out ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
