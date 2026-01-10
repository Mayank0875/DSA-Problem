## Title
Inventory Check

## Slug
inventory-check

## Difficulty
Medium

## Description
A store scans items. 1 is In Stock, 0 is Out of Stock. The manager can emergency order k out-of-stock items.

You scan shelf inventory represented by an array `nums` consisting of 1s (in-stock items) and 0s (missing items), and an integer `k`. You are allowed to restock at most `k` missing itemss from the sequence.

Your task is to find the length of the longest contiguous sequence of in-stock itemss after performing the restocks. If the sequence contains no in-stock itemss even after optimal restocks, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After restocking the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of in-stock itemss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can restock the missing items at index 4 and the missing items at index 7. The resulting segments of in-stock itemss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for in-stock items, 0 for missing items).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of in-stock itemss.

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
