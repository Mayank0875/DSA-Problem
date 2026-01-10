## Title
Space Signal

## Slug
space-signal

## Difficulty
Medium

## Description
A telescope records pulses. 1 is Signal, 0 is Cosmic Noise. An algorithm can filter out k noise pulses.

You analyze radio pulses represented by an array `nums` consisting of 1s (signal pulses) and 0s (noise pulses), and an integer `k`. You are allowed to filter at most `k` noise pulsess from the sequence.

Your task is to find the length of the longest contiguous sequence of signal pulsess after performing the filters. If the sequence contains no signal pulsess even after optimal filters, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After filtering the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of signal pulsess has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can filter the noise pulses at index 4 and the noise pulses at index 7. The resulting segments of signal pulsess merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for signal pulses, 0 for noise pulses).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of signal pulsess.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ nums[i] ≤ 1
- 0 ≤ k ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sliding-window, two-pointers, array

## Company
facebook
