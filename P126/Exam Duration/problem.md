## Title
Exam Duration

## Slug
exam-duration

## Difficulty
Easy

## Description
An online testing platform logs student exam times.

The platform records the start time and submit time of every student in two integer arrays, `startTime` and `endTime`. The $i$-th student begins at `startTime[i]` and submits at `endTime[i]`, inclusive.

The proctor wants to know how many students were taking the exam during a specific server hiccup `[queryStart, queryEnd]`. A student is considered taking the exam if their attempt overlaps with the server hiccup at any point (even for a single moment).

Your task is to return the total number of students who were taking the exam during the given server hiccup.

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
The server hiccup is `[2, 4]`.
- Student 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Student 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Student 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 students were taking the exam.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The student was taking the exam at time `[4, 4]`. The server hiccup is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of students.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of students taking the exam during the server hiccup.

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
