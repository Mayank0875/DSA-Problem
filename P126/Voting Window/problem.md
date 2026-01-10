## Title
Voting Window

## Slug
voting-window

## Difficulty
Easy

## Description
An electronic voting system logs active voting sessions.

The audit log records the session start and session end of every voter in two integer arrays, `startTime` and `endTime`. The $i$-th voter enters the booth at `startTime[i]` and casts vote at `endTime[i]`, inclusive.

The election official wants to know how many voters were voting during a specific lunch break `[queryStart, queryEnd]`. A voter is considered voting if their session overlaps with the lunch break at any point (even for a single moment).

Your task is to return the total number of voters who were voting during the given lunch break.

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
The lunch break is `[2, 4]`.
- Voter 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Voter 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Voter 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 voters were voting.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The voter was voting at time `[4, 4]`. The lunch break is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of voters.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of voters voting during the lunch break.

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
