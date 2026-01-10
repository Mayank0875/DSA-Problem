## Title
Assembly Robot

## Slug
assembly-robot

## Difficulty
Medium

## Description
A robot welds parts. 1 is Strong Weld, 0 is Weak Weld. A supervisor can manually re-weld k weak spots.

You inspect welds represented by an array `nums` consisting of 1s (strong welds) and 0s (weak welds), and an integer `k`. You are allowed to re-weld at most `k` weak weldss from the sequence.

Your task is to find the length of the longest contiguous sequence of strong weldss after performing the fixes. If the sequence contains no strong weldss even after optimal fixes, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After re-welding the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of strong weldss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can re-weld the weak welds at index 4 and the weak welds at index 7. The resulting segments of strong weldss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for strong welds, 0 for weak welds).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of strong weldss.

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
