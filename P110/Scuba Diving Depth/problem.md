## Title
Scuba Diving Depth

## Slug
scuba-diving-depth

## Difficulty
Easy

## Description
A diver descends. A 'Descent Phase' is a sequence of logs where the depth strictly increases.

The Diver is analyzing a sequence of logs represented by an array of integers `nums`, where `nums[i]` represents the depth at index `i`.

The Diver wants to find the maximum total depth obtained during a single "**Descent Phase**". A "Descent Phase" is defined as a contiguous subarray of logs where the depth of each log is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of depths possible from one such Descent Phase. The Descent Phase must include at least one log.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Diver identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Descent Phase starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of logs.
- The second line contains `n` space-separated integers, representing the depths.

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
