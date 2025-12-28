## Title
Subway Maintenance

## Slug
subway-maintenance

## Difficulty
Medium

## Description
Crews work on track sections. Each project covers a start mile marker and end mile marker.

Work orders list list of projects, each defined by a start mile and an end mile, represented as a pair `[start, end]`.

Safety buffers are needed. The end mile of one project must be strictly less than the start mile of the next. Specifically, to transition from project `[a, b]` to a subsequent project `[c, d]`, the end of the first project must be **strictly less than** the start of the second project (i.e., `b < c`).

You can select projects in any order you like to form a valid maintenance plan. Your goal is to determine the maximum number of projects that can be included in a single maintenance plan.

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
The longest maintenance plan is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The projects can be reordered to form the maintenance plan `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available projects.
- The next `n` lines each contain two integers, representing the `start` and `end` of an project.

## Output Format
- Return a single integer representing the maximum length of the maintenance plan.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
