## Title

Next Lower Temperature Day

## Slug

next-lower-temperature-day

## Difficulty

Easy

## Description

You are tracking daily high temperatures in your city. For each day, you're curious about the next upcoming day that will have a strictly lower high temperature. Sometimes, the temperature might only rise or stay the same in the future. 
Given a list of daily high temperatures, your task is to determine, for each day, the temperature of the nearest future day with a lower high temperature. If no such future day exists within the recorded period, indicate that.

## Examples

### 1

#### Input

8
[73, 74, 75, 71, 69, 72, 76, 73]

#### Output

[71, 71, 71, 69, -1, -1, 73, -1]

#### Explanation

Day 0 (73): Next lower is 71 (Day 3). Output 71.
Day 1 (74): Next lower is 71 (Day 3). Output 71.
Day 2 (75): Next lower is 71 (Day 3). Output 71.
Day 3 (71): Next lower is 69 (Day 4). Output 69.
Day 4 (69): No future day is lower. Output -1.
Day 5 (72): The next lower is none. Output -1.
Day 6 (76): Next lower is 73 (Day 7). Output 73.
Day 7 (73): No future day exists. Output -1.

### 2

#### Input

4
[30, 40, 50, 60]

#### Output

[-1, -1, -1, -1]

#### Explanation

Temperatures are strictly increasing, so no future day has a lower temperature.

## Input Format

The first line contains a single integer n, the number of days.
The second line contains n space-separated integers t_0, t_1, ..., t_[n-1], representing the high temperature for each day.

## Output Format

Return array of integers. The i-th integer should be the temperature on the nearest day j > i such that t_j < t_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ t_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array
