## Title

Reverse the Message

## Slug

reverse-the-message

## Difficulty

Medium

## Description

The Communication Center has received a sequence of integers representing a signal. To analyze the data and "reverse" the noise process, you must smooth the signal by calculating local averages.

You are given a **0-indexed** array `nums` of `n` integers and an integer `k`. The **k-radius average** for a subarray centered at index `i` is the average of all elements between indices `i - k` and `i + k` (inclusive).

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

The input string `hello` is modified in-place to become `olleh`.
    
### 2

#### Input

1 
100000 
0

#### Output

100000

#### Explanation

The input string `level` is modified in-place to become `level`.
  

## Input Format  

- The first line contains an integer `n`, representing the number of elements in the array.
- The second line contains `n` space-separated integers representing the array `nums`.
- The third line contains an integer `k`, representing the radius.

## Output Format  

- Return a single line containing `n` space-separated integers, where the `i`-th integer is the k-radius average for index `i`.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 0 ≤ nums[i] ≤ 1e5
- 0 ≤ k ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

two-pointers, array, sliding-window

## Company
facebook