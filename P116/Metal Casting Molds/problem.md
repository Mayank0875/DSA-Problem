## Title
Metal Casting Molds

## Slug
metal-casting-molds

## Difficulty
Medium

## Description
A foundry has molds that operate at specific temperature ranges. Each mold has a min temp and max temp.

The inventory contains list of molds, each defined by a min temp and an max temp, represented as a pair `[min, max]`.

To reuse the alloy cooling process efficiently, the max temp of the current mold must be strictly lower than the min temp of the next mold in the sequence. Specifically, to transition from mold `[a, b]` to a subsequent mold `[c, d]`, the max of the first mold must be **strictly less than** the min of the second mold (i.e., `b < c`).

You can select molds in any order you like to form a valid production line. Your goal is to determine the maximum number of molds that can be included in a single production line.

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
The longest production line is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The molds can be reordered to form the production line `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available molds.
- The next `n` lines each contain two integers, representing the `min` and `max` of an mold.

## Output Format
- Return a single integer representing the maximum length of the production line.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ min < max ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
