## Title

Library Study Session Occupancy

## Slug

library-study-session-occupancy

## Difficulty

Easy

## Description

The university library records the entry and exit times of every student in two integer arrays, `startTime` and `endTime`. The $i$-th student enters at `startTime[i]` and leaves at `endTime[i]`, inclusive.

The head librarian wants to know how many students were present in the library during a specific query interval `[queryStart, queryEnd]`. A student is considered present if their time in the library overlaps with the query interval at any point (even for a single moment).

Your task is to return the total number of students who were studying in the library during the given query interval.

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

The query interval is `[2, 4]`.
- Student 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Student 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Student 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 students were present.
    
### 2

#### Input

1
4
4
1 3

#### Output

0

#### Explanation

The student was present at time `[4, 4]`. The query interval is `[1, 3]`. There is no overlap.
  

## Input Format  

- The first line contains an integer `n`, the number of students.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format  

- Return a single integer representing the number of students present during the query interval.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ startTime[i] ≤ endTime[i] ≤ 1e9
- 1 ≤ queryStart ≤ queryEnd ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, two-pointers

## Company
yandex