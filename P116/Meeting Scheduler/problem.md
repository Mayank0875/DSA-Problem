## Title
Meeting Scheduler

## Slug
meeting-scheduler

## Difficulty
Medium

## Description
An executive wants to attend as many meetings as possible. Each meeting has a start time and an end time.

The schedule has a list of meetings, each defined by a start time and an end time, represented as a pair `[start, end]`.

You cannot attend two meetings at once. To attend a meeting after another, the first meeting must end strictly before the second one begins. Specifically, to transition from meeting `[a, b]` to a subsequent meeting `[c, d]`, the end of the first meeting must be **strictly less than** the start of the second meeting (i.e., `b < c`).

You can select meetings in any order you like to form a valid schedule. Your goal is to determine the maximum number of meetings that can be included in a single schedule.

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
The longest schedule is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The meetings can be reordered to form the schedule `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available meetings.
- The next `n` lines each contain two integers, representing the `start` and `end` of an meeting.

## Output Format
- Return a single integer representing the maximum length of the schedule.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
