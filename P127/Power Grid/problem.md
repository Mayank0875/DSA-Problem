## Title
Power Grid

## Slug
power-grid

## Difficulty
Medium

## Description
A grid monitors stability. 1 is Stable, 0 is Fluctuation. Stabilizers can handle k fluctuations.

You monitor grid status represented by an array `nums` consisting of 1s (stable intervals) and 0s (fluctuations), and an integer `k`. You are allowed to stabilize at most `k` fluctuationss from the sequence.

Your task is to find the length of the longest contiguous sequence of stable intervalss after performing the stabilizers. If the sequence contains no stable intervalss even after optimal stabilizers, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After stabilizing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of stable intervalss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can stabilize the fluctuations at index 4 and the fluctuations at index 7. The resulting segments of stable intervalss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for stable intervals, 0 for fluctuations).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of stable intervalss.

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
