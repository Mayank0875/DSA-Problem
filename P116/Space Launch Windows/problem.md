## Title
Space Launch Windows

## Slug
space-launch-windows

## Difficulty
Medium

## Description
Rockets launch from a single pad. Each mission has a specific launch window start and end time.

The manifest lists list of missions, each defined by a window start and an window end, represented as a pair `[start, end]`.

Safety protocols require the pad to be clear. A mission must end its window strictly before the next mission's window begins. Specifically, to transition from mission `[a, b]` to a subsequent mission `[c, d]`, the end of the first mission must be **strictly less than** the start of the second mission (i.e., `b < c`).

You can select missions in any order you like to form a valid launch schedule. Your goal is to determine the maximum number of missions that can be included in a single launch schedule.

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
The longest launch schedule is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The missions can be reordered to form the launch schedule `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available missions.
- The next `n` lines each contain two integers, representing the `start` and `end` of an mission.

## Output Format
- Return a single integer representing the maximum length of the launch schedule.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
