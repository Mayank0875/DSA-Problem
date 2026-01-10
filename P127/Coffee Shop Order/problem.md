## Title
Coffee Shop Order

## Slug
coffee-shop-order

## Difficulty
Medium

## Description
A barista makes drinks. 1 is Perfect, 0 is Wrong Order. They can remake k wrong orders quickly.

You check drink orders represented by an array `nums` consisting of 1s (perfect drinks) and 0s (wrong orders), and an integer `k`. You are allowed to remake at most `k` wrong orderss from the sequence.

Your task is to find the length of the longest contiguous sequence of perfect drinkss after performing the remakes. If the sequence contains no perfect drinkss even after optimal remakes, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After remaking the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of perfect drinkss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can remake the wrong orders at index 4 and the wrong orders at index 7. The resulting segments of perfect drinkss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for perfect drinks, 0 for wrong orders).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of perfect drinkss.

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
