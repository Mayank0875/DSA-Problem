## Title
Elevator Service

## Slug
elevator-service

## Difficulty
Medium

## Description
An elevator stops at floors. 1 is Operational, 0 is Stuck. A technician can override k stuck instances.

You monitor elevator logs represented by an array `nums` consisting of 1s (operational stops) and 0s (stuck stops), and an integer `k`. You are allowed to override at most `k` stuck stopss from the sequence.

Your task is to find the length of the longest contiguous sequence of operational stopss after performing the overrides. If the sequence contains no operational stopss even after optimal overrides, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After overriding the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of operational stopss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can override the stuck stops at index 4 and the stuck stops at index 7. The resulting segments of operational stopss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for operational stops, 0 for stuck stops).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of operational stopss.

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
