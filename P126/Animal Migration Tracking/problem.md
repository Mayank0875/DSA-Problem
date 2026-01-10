## Title
Animal Migration Tracking

## Slug
animal-migration-tracking

## Difficulty
Easy

## Description
Researchers track animals entering and leaving a protected zone.

The GPS log records the entry day and exit day of every animal in two integer arrays, `startTime` and `endTime`. The $i$-th animal enters the zone at `startTime[i]` and leaves the zone at `endTime[i]`, inclusive.

The biologist wants to know how many animals were in the zone during a specific mating season `[queryStart, queryEnd]`. A animal is considered in the zone if their stay overlaps with the mating season at any point (even for a single moment).

Your task is to return the total number of animals who were in the zone during the given mating season.

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
The mating season is `[2, 4]`.
- Animal 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Animal 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Animal 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 animals were in the zone.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The animal was in the zone at time `[4, 4]`. The mating season is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of animals.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of animals in the zone during the mating season.

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
