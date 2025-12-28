## Title
Climbing Route

## Slug
climbing-route

## Difficulty
Medium

## Description
A climber uses ropes fixed at intervals. Each rope spans from a lower height to a higher height.

The wall has list of ropes, each defined by a bottom and an top, represented as a pair `[bot, top]`.

To transfer safely, the top of the current rope must be strictly lower than the bottom of the next rope (requiring a free climb in between). Specifically, to transition from rope `[a, b]` to a subsequent rope `[c, d]`, the top of the first rope must be **strictly less than** the bot of the second rope (i.e., `b < c`).

You can select ropes in any order you like to form a valid ascent. Your goal is to determine the maximum number of ropes that can be included in a single ascent.

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
The longest ascent is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The ropes can be reordered to form the ascent `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available ropes.
- The next `n` lines each contain two integers, representing the `bot` and `top` of an rope.

## Output Format
- Return a single integer representing the maximum length of the ascent.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ bot < top ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
