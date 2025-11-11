## Title

Sort the Flag

## Slug

sort-the-flag

## Difficulty

Medium

## Description

You are given an array of integers representing a flag of three colors: Red (0), White (1), and Blue (2). Your task is to sort this array in-place so that all the red objects are first, followed by all the white objects, and finally all the blue objects.

You must achieve this without using any built-in sorting functions from your programming library. The sorting must be done by modifying the array directly (in-place) and using only a constant amount of extra memory.

## Examples

### 1

#### Input

6 
[2, 0, 2, 1, 1, 0]

#### Output

[0, 0, 1, 1, 2, 2]

#### Explanation

The array is sorted in-place. All 0s (Red) come first, followed by 1s (White), and then 2s (Blue).
    
### 2

#### Input

3 
[2, 0, 1]

#### Output

[0, 1, 2]

#### Explanation

The input `[2, 0, 1]` is sorted in-place to `[0, 1, 2]`.
  

## Input Format  

- The first line contains an integer n, the number of objects.
- The second line contains $n$ space-separated integers (`nums[i]`), where each integer is 0, 1, or 2.

## Output Format  

- Your function must modify the input array in-place. The printing is handled by the driver code.
  

## Constraints  

- 1 ≤ n ≤ 300
- `nums[i]` is 0, 1, or 2.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

two-pointers, sorting