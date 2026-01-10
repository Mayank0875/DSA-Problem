## Title
Watering System Cycle

## Slug
watering-system-cycle

## Difficulty
Easy

## Description
An automated farm tracks sprinkler activation.

The irrigation log records the on time and off time of every sprinkler in two integer arrays, `startTime` and `endTime`. The $i$-th sprinkler turns on at `startTime[i]` and turns off at `endTime[i]`, inclusive.

The farmer wants to know how many sprinklers were watering during a specific water pressure check `[queryStart, queryEnd]`. A sprinkler is considered watering if their cycle overlaps with the water pressure check at any point (even for a single moment).

Your task is to return the total number of sprinklers who were watering during the given water pressure check.

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
The water pressure check is `[2, 4]`.
- Sprinkler 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Sprinkler 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Sprinkler 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 sprinklers were watering.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The sprinkler was watering at time `[4, 4]`. The water pressure check is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of sprinklers.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of sprinklers watering during the water pressure check.

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
