## Title
Heart Rate Zone

## Slug
heart-rate-zone

## Difficulty
Easy

## Description
A runner monitors their pulse. An 'Exertion Spike' is a period where their heart rate strictly rises every interval.

The Runner is analyzing a sequence of intervals represented by an array of integers `nums`, where `nums[i]` represents the BPM at index `i`.

The Runner wants to find the maximum total BPM obtained during a single "**Exertion Spike**". A "Exertion Spike" is defined as a contiguous subarray of intervals where the BPM of each interval is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of BPMs possible from one such Exertion Spike. The Exertion Spike must include at least one interval.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Runner identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Exertion Spike starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of intervals.
- The second line contains `n` space-separated integers, representing the BPMs.

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
