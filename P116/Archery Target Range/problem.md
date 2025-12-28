## Title
Archery Target Range

## Slug
archery-target-range

## Difficulty
Medium

## Description
Archers shoot at targets placed at different distance intervals. Each target occupies a range of depth.

The field has list of targets, each defined by a front depth and an back depth, represented as a pair `[front, back]`.

An arrow flying through needs clear space. The back depth of one target must be strictly less than the front depth of the next. Specifically, to transition from target `[a, b]` to a subsequent target `[c, d]`, the back of the first target must be **strictly less than** the front of the second target (i.e., `b < c`).

You can select targets in any order you like to form a valid shot line. Your goal is to determine the maximum number of targets that can be included in a single shot line.

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
The longest shot line is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The targets can be reordered to form the shot line `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available targets.
- The next `n` lines each contain two integers, representing the `front` and `back` of an target.

## Output Format
- Return a single integer representing the maximum length of the shot line.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ front < back ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
