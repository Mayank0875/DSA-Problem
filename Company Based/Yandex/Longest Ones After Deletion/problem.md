## Title

Longest Ones After Deletion

## Slug

longest-ones-after-deletion

## Difficulty

Medium

## Description

You are given a binary array `nums` consisting of 0s and 1s, and an integer `k`. You are allowed to delete at most `k` elements from the array.

Your task is to find the length of the longest contiguous subarray containing only 1s after performing the deletions. If the array contains no 1s even after optimal deletions, return 0.

## Examples

### 1

#### Input

4 
1 1 0 1
1

#### Output

3

#### Explanation

After deleting the number at position 2 (value 0), the array becomes `[1, 1, 1]`. The longest subarray of 1s has length 3.
    
### 2

#### Input

9
0 1 1 1 0 1 1 0 1
2

#### Output

6

#### Explanation

We can delete the 0 at index 4 and the 0 at index 7. The resulting segments of 1s merge to form a sequence of length 6.
  

## Input Format  

- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the binary array `nums`.
- The third line contains an integer `k`.

## Output Format  

- Return a single integer representing the maximum size of the subarray of 1s.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 0 ≤ nums[i] ≤ 1
- 1 ≤ k ≤ n

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sliding-window, two-pointers, array

## Company
yandex