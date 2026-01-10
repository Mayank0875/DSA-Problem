## Title
Signal Reception

## Slug
signal-reception

## Difficulty
Medium

## Description
A radio receiver gets bits. 1 is Clear, 0 is Static. A noise filter can clean up k static bits.

You receive a signal stream represented by an array `nums` consisting of 1s (clear signals) and 0s (static bursts), and an integer `k`. You are allowed to filter at most `k` static burstss from the sequence.

Your task is to find the length of the longest contiguous sequence of clear signalss after performing the filters. If the sequence contains no clear signalss even after optimal filters, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After filtering the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of clear signalss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can filter the static bursts at index 4 and the static bursts at index 7. The resulting segments of clear signalss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for clear signals, 0 for static bursts).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of clear signalss.

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
