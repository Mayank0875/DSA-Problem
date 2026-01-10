## Title
Solar Panel Efficiency

## Slug
solar-panel-efficiency

## Difficulty
Medium

## Description
Panels generate power hourly. 1 is High Output, 0 is Low Output (Cloudy). Batteries can compensate for k low-output hours.

You track energy generation represented by an array `nums` consisting of 1s (high output hours) and 0s (low output hours), and an integer `k`. You are allowed to compensate for at most `k` low output hourss from the sequence.

Your task is to find the length of the longest contiguous sequence of high output hourss after performing the compensations. If the sequence contains no high output hourss even after optimal compensations, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After compensating for the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of high output hourss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can compensate for the low output hours at index 4 and the low output hours at index 7. The resulting segments of high output hourss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for high output hours, 0 for low output hours).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of high output hourss.

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
