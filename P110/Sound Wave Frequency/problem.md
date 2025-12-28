## Title
Sound Wave Frequency

## Slug
sound-wave-frequency

## Difficulty
Easy

## Description
An audio engineer analyzes a chirp signal. A 'Sweep Up' is a sequence of samples where the frequency strictly increases.

The Engineer is analyzing a sequence of samples represented by an array of integers `nums`, where `nums[i]` represents the frequency at index `i`.

The Engineer wants to find the maximum total frequency obtained during a single "**Sweep Up**". A "Sweep Up" is defined as a contiguous subarray of samples where the frequency of each sample is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of frequencys possible from one such Sweep Up. The Sweep Up must include at least one sample.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Engineer identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Sweep Up starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of samples.
- The second line contains `n` space-separated integers, representing the frequencys.

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
