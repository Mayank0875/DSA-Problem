## Title
Crescendo Master

## Slug
crescendo-master

## Difficulty
Easy

## Description
A conductor leads an orchestra. A 'Perfect Crescendo' is a sequence of measures where the volume (decibels) strictly increases.

The Conductor is analyzing a sequence of measures represented by an array of integers `nums`, where `nums[i]` represents the decibel level at index `i`.

The Conductor wants to find the maximum total decibel level obtained during a single "**Perfect Crescendo**". A "Perfect Crescendo" is defined as a contiguous subarray of measures where the decibel level of each measure is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of decibel levels possible from one such Perfect Crescendo. The Perfect Crescendo must include at least one measure.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Conductor identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Perfect Crescendo starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of measures.
- The second line contains `n` space-separated integers, representing the decibel levels.

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
