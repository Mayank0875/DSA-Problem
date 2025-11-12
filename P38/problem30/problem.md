## Title

Previous Lower Digital Ruin Level

## Slug

previous-lower-digital-ruins

## Difficulty

Easy

## Description

You are exploring a series of ancient digital ruins, where each segment records a signal intensity. For each segment, you need to determine the intensity recorded at the nearest previous segment that had a strictly lower intensity than the current one. If no such previous segment exists (either because it is the first segment or all earlier intensities are higher or equal), you should indicate this. This information helps archaeologists understand the degradation patterns within the ruins. Your task is to compute this value for every segment given the sequence of signal intensities.

## Examples

### 1

#### Input

8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output

[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation

Day 0 (100): No previous segment, output -1.
Day 1 (80): Intensity 100 on day 0 is not lower, output -1.
Day 2 (60): Intensities 100, 80 are not lower, output -1.
Day 3 (70): Intensity 60 on day 2 is lower, output 60.
Day 4 (60): Intensities 100, 80, 60, 70. None are strictly lower, output -1.
Day 5 (75): Intensity 60 on day 4 is the nearest lower, output 60.
Day 6 (85): Intensity 75 on day 5 is the nearest lower, output 75.
Day 7 (110): Intensity 85 on day 6 is the nearest lower, output 85.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All intensities are equal, so no strictly lower previous intensity exists for any segment.

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