## Title

Echoes of Infinity

## Slug

echoes-of-infinity

## Difficulty

Easy

## Description

You are studying the resonant patterns of an ancient cosmic phenomenon known as the **Echoes of Infinity**. At each moment in time, an echo is recorded with a certain intensity. For every recorded echo, you need to determine the intensity of the nearest earlier echo whose intensity was strictly lower than the current one. If there is no such earlier echo (either because it is the first recorded moment or all previous intensities are higher or equal), you should indicate this with `-1`. This analysis helps uncover the underlying decay structure of the infinite echo sequence. Your task is to compute this value for every moment given the sequence of echo intensities.

## Examples

### 1

#### Input

8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output

[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation

Moment 0 (100): No previous echo, output -1.  
Moment 1 (80): Intensity 100 at moment 0 is not lower, output -1.  
Moment 2 (60): Intensities 100, 80 are not lower, output -1.  
Moment 3 (70): Intensity 60 at moment 2 is lower, output 60.  
Moment 4 (60): Intensities 100, 80, 60, 70. None are strictly lower, output -1.  
Moment 5 (75): Intensity 60 at moment 4 is the nearest lower, output 60.  
Moment 6 (85): Intensity 75 at moment 5 is the nearest lower, output 75.  
Moment 7 (110): Intensity 85 at moment 6 is the nearest lower, output 85.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All intensities are equal, so no strictly lower previous echo exists for any moment.

## Input Format

The first line contains a single integer n, the number of moments.  
The second line contains n space-separated integers p_0, p_1, ..., p_[n-1], representing the echo intensity for each moment.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest moment j < i such that p_j < p_i. If no such moment exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ p_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array