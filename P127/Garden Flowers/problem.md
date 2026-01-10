## Title
Garden Flowers

## Slug
garden-flowers

## Difficulty
Medium

## Description
A flower bed row has plants. 1 is Blooming, 0 is Withered. The gardener can replace k withered plants to make a continuous bloom.

You inspect a flower bed represented by an array `nums` consisting of 1s (blooming flowers) and 0s (withered flowers), and an integer `k`. You are allowed to replace at most `k` withered flowerss from the sequence.

Your task is to find the length of the longest contiguous sequence of blooming flowerss after performing the replacements. If the sequence contains no blooming flowerss even after optimal replacements, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After replacing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of blooming flowerss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can replace the withered flowers at index 4 and the withered flowers at index 7. The resulting segments of blooming flowerss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for blooming flowers, 0 for withered flowers).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of blooming flowerss.

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
