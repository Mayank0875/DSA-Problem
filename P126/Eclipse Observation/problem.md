## Title
Eclipse Observation

## Slug
eclipse-observation

## Difficulty
Easy

## Description
Astronomers track when different observatories can see an eclipse.

The visibility chart records the start visibility and end visibility of every observatory in two integer arrays, `startTime` and `endTime`. The $i$-th observatory starts seeing the eclipse at `startTime[i]` and stops seeing it at `endTime[i]`, inclusive.

The coordinator wants to know how many observatories were observing during a specific totality phase `[queryStart, queryEnd]`. A observatory is considered observing if their viewing window overlaps with the totality phase at any point (even for a single moment).

Your task is to return the total number of observatories who were observing during the given totality phase.

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
The totality phase is `[2, 4]`.
- Observatory 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Observatory 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Observatory 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 observatories were observing.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The observatory was observing at time `[4, 4]`. The totality phase is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of observatories.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of observatories observing during the totality phase.

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
