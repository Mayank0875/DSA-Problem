## Title
Fireworks Finale

## Slug
fireworks-finale

## Difficulty
Easy

## Description
A pyrotechnician designs a show. The 'Grand Finale' is a sequence where the number of explosions per second strictly increases.

The Pyrotechnician is analyzing a sequence of seconds represented by an array of integers `nums`, where `nums[i]` represents the explosion count at index `i`.

The Pyrotechnician wants to find the maximum total explosion count obtained during a single "**Grand Finale**". A "Grand Finale" is defined as a contiguous subarray of seconds where the explosion count of each second is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of explosion counts possible from one such Grand Finale. The Grand Finale must include at least one second.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Pyrotechnician identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Grand Finale starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of seconds.
- The second line contains `n` space-separated integers, representing the explosion counts.

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
