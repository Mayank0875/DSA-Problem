## Title
Daily Sales Momentum

## Slug
daily-sales-momentum

## Difficulty
Medium

## Description
A store manager tracks daily revenue. They define 'sales momentum' for a given day as the count of consecutive days ending on that day (including itself) where the revenue was less than or equal to the current day's revenue. This helps identify local peaks in performance. Given the daily sales figures, calculate the momentum for each day.

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
