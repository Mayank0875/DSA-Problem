## Title
Restaurant Reservation

## Slug
restaurant-reservation

## Difficulty
Easy

## Description
A restaurant tracks table occupancy.

The reservation book records the seating time and departure time of every party in two integer arrays, `startTime` and `endTime`. The $i$-th party is seated at `startTime[i]` and leaves at `endTime[i]`, inclusive.

The host wants to know how many parties were dining during a specific dinner rush `[queryStart, queryEnd]`. A party is considered dining if their meal overlaps with the dinner rush at any point (even for a single moment).

Your task is to return the total number of parties who were dining during the given dinner rush.

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
The dinner rush is `[2, 4]`.
- Party 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Party 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Party 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 parties were dining.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The party was dining at time `[4, 4]`. The dinner rush is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of parties.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of parties dining during the dinner rush.

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
