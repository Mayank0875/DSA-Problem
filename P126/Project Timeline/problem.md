## Title
Project Timeline

## Slug
project-timeline

## Difficulty
Easy

## Description
A project manager tracks task durations.

The Gantt chart records the start date and end date of every task in two integer arrays, `startTime` and `endTime`. The $i$-th task starts at `startTime[i]` and completes at `endTime[i]`, inclusive.

The PM wants to know how many tasks were in progress during a specific critical week `[queryStart, queryEnd]`. A task is considered in progress if their duration overlaps with the critical week at any point (even for a single moment).

Your task is to return the total number of tasks who were in progress during the given critical week.

## Examples

### 1

#### Input
3
1 2 3
3 2 7
2 4

#### Output
3

#### Explanation
The critical week is `[2, 4]`.
- Task 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Task 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Task 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 tasks were in progress.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The task was in progress at time `[4, 4]`. The critical week is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of tasks.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of tasks in progress during the critical week.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ startTime[i] ≤ endTime[i] ≤ 10^9
- 1 ≤ queryStart ≤ queryEnd ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, interval, linear-scan

## Company
amazon
