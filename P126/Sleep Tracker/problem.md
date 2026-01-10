## Title
Sleep Tracker

## Slug
sleep-tracker

## Difficulty
Easy

## Description
A health app logs sleep cycles.

The user data records the sleep onset and wake time of every user in two integer arrays, `startTime` and `endTime`. The $i$-th user falls asleep at `startTime[i]` and wakes up at `endTime[i]`, inclusive.

The researcher wants to know how many users were asleep during a specific REM window `[queryStart, queryEnd]`. A user is considered asleep if their sleep overlaps with the REM window at any point (even for a single moment).

Your task is to return the total number of users who were asleep during the given REM window.

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
The REM window is `[2, 4]`.
- User 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- User 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- User 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 users were asleep.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The user was asleep at time `[4, 4]`. The REM window is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of users.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of users asleep during the REM window.

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
