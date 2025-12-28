## Title
Security Guard Patrol

## Slug
security-guard-patrol

## Difficulty
Medium

## Description
A guard checks zones. Each zone occupies a time interval to inspect.

The duty roster has list of zones, each defined by a start time and an end time, represented as a pair `[start, end]`.

The guard is one person. They must finish a zone strictly before starting the next. Specifically, to transition from zone `[a, b]` to a subsequent zone `[c, d]`, the end of the first zone must be **strictly less than** the start of the second zone (i.e., `b < c`).

You can select zones in any order you like to form a valid patrol. Your goal is to determine the maximum number of zones that can be included in a single patrol.

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
The longest patrol is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The zones can be reordered to form the patrol `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available zones.
- The next `n` lines each contain two integers, representing the `start` and `end` of an zone.

## Output Format
- Return a single integer representing the maximum length of the patrol.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
