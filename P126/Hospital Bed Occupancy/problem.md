## Title
Hospital Bed Occupancy

## Slug
hospital-bed-occupancy

## Difficulty
Easy

## Description
A hospital manages patient admissions and discharges.

The registry records the admission day and discharge day of every patient in two integer arrays, `startTime` and `endTime`. The $i$-th patient is admitted at `startTime[i]` and is discharged at `endTime[i]`, inclusive.

The head nurse wants to know how many patients were occupying a bed during a specific audit week `[queryStart, queryEnd]`. A patient is considered occupying a bed if their stay overlaps with the audit week at any point (even for a single moment).

Your task is to return the total number of patients who were occupying a bed during the given audit week.

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
The audit week is `[2, 4]`.
- Patient 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Patient 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Patient 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 patients were occupying a bed.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The patient was occupying a bed at time `[4, 4]`. The audit week is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of patients.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of patients occupying a bed during the audit week.

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
