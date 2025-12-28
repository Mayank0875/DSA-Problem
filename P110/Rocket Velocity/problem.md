## Title
Rocket Velocity

## Slug
rocket-velocity

## Difficulty
Easy

## Description
Mission control monitors a rocket. A 'Thrust Phase' is a period where the rocket's velocity increases strictly every second.

Mission Control is analyzing a sequence of velocity readings represented by an array of integers `nums`, where `nums[i]` represents the speed unit at index `i`.

Mission Control wants to find the maximum total speed unit obtained during a single "**Thrust Phase**". A "Thrust Phase" is defined as a contiguous subarray of velocity readings where the speed unit of each reading is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of speed units possible from one such Thrust Phase. The Thrust Phase must include at least one reading.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The Mission Control identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Thrust Phase starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of velocity readings.
- The second line contains `n` space-separated integers, representing the speed units.

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
