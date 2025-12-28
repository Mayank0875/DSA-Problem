## Title
Robot Arm Welding

## Slug
robot-arm-welding

## Difficulty
Medium

## Description
A robot welds seams. Each seam spans a start coordinate and end coordinate.

The blueprint shows list of seams, each defined by a start and an end, represented as a pair `[s, e]`.

The robot moves linearly. It must finish one seam strictly before reaching the start of the next. Specifically, to transition from seam `[a, b]` to a subsequent seam `[c, d]`, the e of the first seam must be **strictly less than** the s of the second seam (i.e., `b < c`).

You can select seams in any order you like to form a valid weld path. Your goal is to determine the maximum number of seams that can be included in a single weld path.

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
The longest weld path is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The seams can be reordered to form the weld path `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available seams.
- The next `n` lines each contain two integers, representing the `s` and `e` of an seam.

## Output Format
- Return a single integer representing the maximum length of the weld path.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ s < e ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
