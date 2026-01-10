## Title
Drone Flight

## Slug
drone-flight

## Difficulty
Medium

## Description
A drone flies checkpoints. 1 is Reached, 0 is Missed. The GPS can guide it to recover k missed points.

You track drone checkpoints represented by an array `nums` consisting of 1s (reached points) and 0s (missed points), and an integer `k`. You are allowed to recover at most `k` missed pointss from the sequence.

Your task is to find the length of the longest contiguous sequence of reached pointss after performing the recoveries. If the sequence contains no reached pointss even after optimal recoveries, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After recovering the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of reached pointss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can recover the missed points at index 4 and the missed points at index 7. The resulting segments of reached pointss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for reached points, 0 for missed points).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of reached pointss.

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
