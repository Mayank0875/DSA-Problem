## Title
CPU Job Scheduling

## Slug
cpu-job-scheduling

## Difficulty
Medium

## Description
A single-core CPU receives jobs. Each job requires a start cycle and end cycle.

The queue contains list of jobs, each defined by a start cycle and an end cycle, represented as a pair `[start, end]`.

The CPU cannot multitask. A job must finish strictly before the next one starts. Specifically, to transition from job `[a, b]` to a subsequent job `[c, d]`, the end of the first job must be **strictly less than** the start of the second job (i.e., `b < c`).

You can select jobs in any order you like to form a valid execution order. Your goal is to determine the maximum number of jobs that can be included in a single execution order.

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
The longest execution order is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The jobs can be reordered to form the execution order `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available jobs.
- The next `n` lines each contain two integers, representing the `start` and `end` of an job.

## Output Format
- Return a single integer representing the maximum length of the execution order.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
