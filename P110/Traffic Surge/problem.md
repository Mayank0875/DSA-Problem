## Title
Traffic Surge

## Slug
traffic-surge

## Difficulty
Easy

## Description
A city planner studies traffic density. A 'Rush Hour Surge' is a time window where the number of cars passing strictly increases every minute.

The Planner is analyzing a sequence of minute logs represented by an array of integers `nums`, where `nums[i]` represents the car count at index `i`.

The Planner wants to find the maximum total car count obtained during a single "**Rush Hour Surge**". A "Rush Hour Surge" is defined as a contiguous subarray of minute logs where the car count of each minute is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of car counts possible from one such Rush Hour Surge. The Rush Hour Surge must include at least one minute.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Planner identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Rush Hour Surge starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of minute logs.
- The second line contains `n` space-separated integers, representing the car counts.

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
