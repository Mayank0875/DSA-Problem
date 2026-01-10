## Title
Car Rental Period

## Slug
car-rental-period

## Difficulty
Easy

## Description
A rental agency tracks fleet usage.

The booking system records the pickup and return of every vehicle in two integer arrays, `startTime` and `endTime`. The $i$-th vehicle is picked up at `startTime[i]` and is returned at `endTime[i]`, inclusive.

The fleet manager wants to know how many vehicles were rented out during a specific holiday season `[queryStart, queryEnd]`. A vehicle is considered rented out if their rental overlaps with the holiday season at any point (even for a single moment).

Your task is to return the total number of vehicles who were rented out during the given holiday season.

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
The holiday season is `[2, 4]`.
- Vehicle 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Vehicle 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Vehicle 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 vehicles were rented out.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The vehicle was rented out at time `[4, 4]`. The holiday season is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of vehicles.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of vehicles rented out during the holiday season.

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
