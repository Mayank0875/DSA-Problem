## Title
Employee Work Hours

## Slug
employee-work-hours

## Difficulty
Easy

## Description
HR tracks employee working hours.

The timesheet records the clock-in and clock-out of every employee in two integer arrays, `startTime` and `endTime`. The $i$-th employee starts at `startTime[i]` and finishes at `endTime[i]`, inclusive.

The HR manager wants to know how many employees were working during a specific core hours `[queryStart, queryEnd]`. A employee is considered working if their shift overlaps with the core hours at any point (even for a single moment).

Your task is to return the total number of employees who were working during the given core hours.

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
The core hours is `[2, 4]`.
- Employee 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Employee 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Employee 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 employees were working.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The employee was working at time `[4, 4]`. The core hours is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of employees.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of employees working during the core hours.

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
