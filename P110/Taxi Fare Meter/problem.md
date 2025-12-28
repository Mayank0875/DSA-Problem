## Title
Taxi Fare Meter

## Slug
taxi-fare-meter

## Difficulty
Easy

## Description
A taxi driver reviews trip fares. A 'Golden Shift' is a sequence of trips where each fare is strictly higher than the last.

The Driver is analyzing a sequence of trips represented by an array of integers `nums`, where `nums[i]` represents the fare amount at index `i`.

The Driver wants to find the maximum total fare amount obtained during a single "**Golden Shift**". A "Golden Shift" is defined as a contiguous subarray of trips where the fare amount of each trip is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of fare amounts possible from one such Golden Shift. The Golden Shift must include at least one trip.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Driver identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Golden Shift starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of trips.
- The second line contains `n` space-separated integers, representing the fare amounts.

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
