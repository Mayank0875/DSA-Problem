## Title

Bitstream Echo

## Slug

bitstream-echo

## Difficulty

Easy

## Description

You are examining a digital bitstream where each element represents the amplitude of a signal at a successive time step. For every position in the stream, you need to determine the amplitude of the nearest previous element that is **strictly lower** than the current amplitude. If such a previous element does not exist (either because it is the first element or all earlier amplitudes are greater than or equal to the current one), you should indicate this with `-1`. This information helps identify the most recent lower echo in the bitstream. Compute this value for every position given the sequence of amplitudes.

## Examples

### 1

#### Input

8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output

[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation

Day 0 (100): No previous element, output -1.  
Day 1 (80): Amplitude 100 on day 0 is not lower, output -1.  
Day 2 (60): Amplitudes 100, 80 are not lower, output -1.  
Day 3 (70): Amplitude 60 on day 2 is lower, output 60.  
Day 4 (60): Amplitudes 100, 80, 60, 70. None are strictly lower, output -1.  
Day 5 (75): Amplitude 60 on day 4 is the nearest lower, output 60.  
Day 6 (85): Amplitude 75 on day 5 is the nearest lower, output 75.  
Day 7 (110): Amplitude 85 on day 6 is the nearest lower, output 85.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All amplitudes are equal, so no strictly lower previous amplitude exists for any position.

## Input Format

The first line contains a single integer n, the number of days.  
The second line contains n space-separated integers p_0, p_1, ..., p_[n-1], representing the amplitude for each position.

## Output Format

Return array of integers. The i-th integer should be the amplitude on the nearest position j < i such that p_j < p_i. If no such position exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ p_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array