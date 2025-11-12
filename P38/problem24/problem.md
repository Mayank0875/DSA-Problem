## Title

Memory Fracture

## Slug

memory-fracture

## Difficulty

Easy

## Description

You are studying a series of neural activation levels recorded over consecutive time steps in a subject experiencing memory fractures. For each time step, you need to determine the activation level at the nearest previous step where the activation was strictly lower than the current level. If no such previous step exists (either because it's the first step or all earlier activations were higher or equal), you should indicate this. This analysis helps identify moments when the subject's memory was less engaged before a surge. Your task is to compute this value for every time step given the activation levels.

## Examples

### 1

#### Input

8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output

[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation

Day 0 (100): No previous day, output -1.
Day 1 (80): Price 100 on day 0 is not lower, output -1.
Day 2 (60): Prices 100, 80 are not lower, output -1.
Day 3 (70): Price 60 on day 2 is lower, output 60.
Day 4 (60): Prices 100, 80, 60, 70. None are strictly lower, output -1.
Day 5 (75): Price 60 on day 4 is the nearest lower, output 60.
Day 6 (85): Price 75 on day 5 is the nearest lower, output 75.
Day 7 (110): Price 85 on day 6 is the nearest lower, output 85.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All prices are equal, so no strictly lower previous price exists for any day.

## Input Format

The first line contains a single integer n, the number of days.
The second line contains n space-separated integers p_0, p_1, ..., p_[n-1], representing the stock price for each day.

## Output Format

Return array of integers. The i-th integer should be the stock price on the nearest day j < i such that p_j < p_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ p_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array