## Title
Fishing Trip

## Slug
fishing-trip

## Difficulty
Medium

## Description
A fisherman casts a line. 1 is Catch, 0 is Empty. They can use k pieces of special bait to turn empty casts into catches.

You log casting results represented by an array `nums` consisting of 1s (catches) and 0s (empty casts), and an integer `k`. You are allowed to bait at most `k` empty castss from the sequence.

Your task is to find the length of the longest contiguous sequence of catchess after performing the baits. If the sequence contains no catchess even after optimal baits, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After baiting the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of catchess has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can bait the empty casts at index 4 and the empty casts at index 7. The resulting segments of catchess merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for catches, 0 for empty casts).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of catchess.

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
