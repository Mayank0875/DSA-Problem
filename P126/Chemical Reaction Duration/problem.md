## Title
Chemical Reaction Duration

## Slug
chemical-reaction-duration

## Difficulty
Easy

## Description
A lab monitors concurrent chemical reactions.

The experiment log records the reaction start and reaction end of every reaction in two integer arrays, `startTime` and `endTime`. The $i$-th reaction begins at `startTime[i]` and completes at `endTime[i]`, inclusive.

The chemist wants to know how many reactions were active during a specific temperature spike `[queryStart, queryEnd]`. A reaction is considered active if their process overlaps with the temperature spike at any point (even for a single moment).

Your task is to return the total number of reactions who were active during the given temperature spike.

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
The temperature spike is `[2, 4]`.
- Reaction 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Reaction 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Reaction 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 reactions were active.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The reaction was active at time `[4, 4]`. The temperature spike is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of reactions.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of reactions active during the temperature spike.

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
