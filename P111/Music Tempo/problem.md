## Title
Music Tempo

## Slug
music-tempo

## Difficulty
Medium

## Description
DJ software detects BPM. It averages the time between beats to provide a stable tempo reading for mixing.

You are given a **0-indexed** array `nums` of `n` integers representing beat intervals and an integer `k`.

The **k-radius average** for a subarray centered at index `i` is the average of all elements between indices `i - k` and `i + k` (inclusive).

If index `i` has fewer than `k` elements before or after it, the average is considered `-1`. Otherwise, the average is the sum of the `2k + 1` elements divided by `2k + 1`, using **integer division** (truncating toward zero).

Your task is to build and return an array where the `i`-th element is the k-radius average of the subarray centered at `i`.

## Examples

### 1

#### Input
9 
7 4 3 9 1 8 5 2 6 
3

#### Output
-1 -1 -1 5 4 4 -1 -1 -1

#### Explanation
- For index 3: The subarray is `[7, 4, 3, 9, 1, 8, 5]`. Sum is 37. Average is `37 // 7 = 5`.
- For index 4: The subarray is `[4, 3, 9, 1, 8, 5, 2]`. Sum is 32. Average is `32 // 7 = 4`.
- For index 5: The subarray is `[3, 9, 1, 8, 5, 2, 6]`. Sum is 34. Average is `34 // 7 = 4`.
- Indices 0, 1, 2 and 6, 7, 8 do not have enough neighbors, so they are `-1`.

### 2

#### Input
1 
100000 
0

#### Output
100000

#### Explanation
With k=0, the average is just the element itself.

## Input Format
- The first line contains an integer `n`, representing the number of beat intervals.
- The second line contains `n` space-separated integers representing the array `nums`.
- The third line contains an integer `k`, representing the radius.

## Output Format
- Return a single line containing `n` space-separated integers, where the `i`-th integer is the k-radius average for index `i`.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ nums[i] ≤ 10^5
- 0 ≤ k ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, sliding-window

