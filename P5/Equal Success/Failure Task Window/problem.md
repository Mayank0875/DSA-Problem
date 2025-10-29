## Title

Equal Success/Failure Task Window

## Slug

equal-success-failure-task-window

## Difficulty

Easy

## Description

A log records the outcome of N consecutive automated tasks, with '1' indicating success and '0' indicating failure. We need to find the longest continuous window of tasks in this log where the number of successful tasks is equal to the number of failed tasks. This helps identify periods of consistent but mixed performance. Given the task outcome log, find the length of the longest such window.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The window [0, 1] (Failure, Success) is the longest with an equal number of successes and failures.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] (Failure, Success) and [1, 0] (Success, Failure) are the longest balanced windows.

## Input Format

- The first line contains a single integer N, the total number of tasks logged.
- The second line contains N space-separated integers, representing task outcomes (0 for failure, 1 for success).

## Output Format

- Return a single integer representing the length of the longest contiguous window with an equal number of 0s and 1s.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, data analysis, prefix sum, hashmap