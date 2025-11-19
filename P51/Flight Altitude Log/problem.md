## Title
Flight Altitude Log

## Slug
flight-altitude-log

## Difficulty
Medium

## Description
A black box records the altitude of a plane at fixed intervals. For each interval, the system calculates an 'altitude streak', which is the number of consecutive previous intervals (including the current one) where the altitude was less than or equal to the current reading. Given the altitude data, calculate this streak.

## Examples

### 1

#### Input
7
100 80 60 70 60 75 85

#### Output
1 1 1 2 1 4 6

#### Explanation
Index 0 (100): Streak is 1.
Index 1 (80): Streak is 1.
Index 2 (60): Streak is 1.
Index 3 (70): 60 <= 70. Streak is 2.
Index 4 (60): Streak is 1.
Index 5 (75): 60, 70, 60 <= 75. Streak is 4.
Index 6 (85): 80, 60, 70, 60, 75 <= 85. Streak is 6.

### 2

#### Input
5
10 20 30 40 50

#### Output
1 2 3 4 5

#### Explanation
Each value is greater than all previous values, so the streak increments by 1 each step.

## Input Format
- The first line contains a single integer n, the number of entries.
- The second line contains n space-separated integers, representing the data sequence.

## Output Format
- Return an n-sized array, where the i-th integer is the streak for index i.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ value ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, array
