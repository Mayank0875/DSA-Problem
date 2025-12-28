## Title
Staircase Sprints

## Slug
staircase-sprints

## Difficulty
Easy

## Description
An athlete is running up flights of stairs. A 'Power Sprint' occurs when they climb consecutive flights, taking strictly more steps on each subsequent flight.

The Athlete is analyzing a sequence of flights represented by an array of integers `nums`, where `nums[i]` represents the step count at index `i`.

The Athlete wants to find the maximum total step count obtained during a single "**Power Sprint**". A "Power Sprint" is defined as a contiguous subarray of flights where the step count of each flight is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of step counts possible from one such Power Sprint. The Power Sprint must include at least one flight.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Athlete identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Power Sprint starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of flights.
- The second line contains `n` space-separated integers, representing the step counts.

## Output Format
- Return a single integer representing the maximum sum of any strictly increasing contiguous subarray.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ nums[i] ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sliding-window, easy
