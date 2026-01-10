## Title
Subway Commute

## Slug
subway-commute

## Difficulty
Medium

## Description
A commuter takes the train. 1 is On Time, 0 is Delayed. They have k 'excuse slips' for being late due to delays.

You log commute times represented by an array `nums` consisting of 1s (on-time arrivals) and 0s (delays), and an integer `k`. You are allowed to excuse at most `k` delayss from the sequence.

Your task is to find the length of the longest contiguous sequence of on-time arrivalss after performing the excuses. If the sequence contains no on-time arrivalss even after optimal excuses, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After excusing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of on-time arrivalss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can excuse the delays at index 4 and the delays at index 7. The resulting segments of on-time arrivalss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for on-time arrivals, 0 for delays).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of on-time arrivalss.

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
