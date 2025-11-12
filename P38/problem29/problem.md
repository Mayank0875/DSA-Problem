## Title

Fractal Current

## Slug

fractal-current

## Difficulty

Easy

## Description

You're analyzing a sequence of measurements of a fractal current at successive points. For each point, you want to find the current value at the nearest previous point where the current was strictly lower than the current point's value. If no such previous point exists (either because it's the first point or all previous values were higher or equal), you should indicate this. This analysis helps understand recent drops in the fractal current. Your task is to compute this value for every point given the sequence of current measurements.

## Examples

### 1

#### Input

8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output

[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation

Day 0 (100): No previous point, output -1.
Day 1 (80): Value 100 on day 0 is not lower, output -1.
Day 2 (60): Values 100, 80 are not lower, output -1.
Day 3 (70): Value 60 on day 2 is lower, output 60.
Day 4 (60): Values 100, 80, 60, 70. None are strictly lower, output -1.
Day 5 (75): Value 60 on day 4 is the nearest lower, output 60.
Day 6 (85): Value 75 on day 5 is the nearest lower, output 75.
Day 7 (110): Value 85 on day 6 is the nearest lower, output 85.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All values are equal, so no strictly lower previous value exists for any point.

## Input Format

The first line contains a single integer n, the number of points.
The second line contains n space-separated integers p_0, p_1, ..., p_[n-1], representing the current measurement for each point.

## Output Format

Return array of integers. The i-th integer should be the current value on the nearest point j < i such that p_j < p_i. If no such point exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ p_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array